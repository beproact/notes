#### Program vs Process
Program is the instructions to do something.
Process is program + state.





Having multiple processes occurring at once.

Multitasking


#### Process Control Block
```c

enum state_type {new,ready,running, waiting, halted};


typedef struct control_block_type {
	enum state_type state;
	address PC; //where to resume
	int reg_file[NUMREGS]; // reg contents
	struct control_block *next_pcb; 
	int priority; //extrinsic attibute
	address memory_footprint; // memory occupancy
	...,
	...,
} control_block;
```

Ready Queue
IO Queue

Scheduler's Job is to order the queue. 


##### Steps for Scheduler
Grab attention of processor
Save the state
Select a new process
Dispatch selected process

###### Preemptive vs Non-Preemptive
Preemptive Comes from external interupt

Non-Preemptive comes from trap, IO request or process exit.


Thrashing- Spending all time switching between processess and exceeds memory capacity of the system.


Non_Preemptive Scheduling Algorithms
FCFS
SJF

Priority

