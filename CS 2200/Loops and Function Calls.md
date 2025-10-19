##### ISA for loops
Conditional and unconditional branches are sufficient

```asm
loop beq r1 r0 done
	loop body
	beq r0 r0 loop
```



##### Function Calls
Branch out and run something else

Pass parameters 
Remember return addr
Jump to procedure
Calling Conventions basically

	JALR r_target r_link
r_target is where we jump to
r_link is where we store the return address to



J r_target
jumps to address in r_target
zero register always returns zero and if written to just reverts back to zero
JALR r_target $zero

API
Call return

##### Shadow Register
Different sets of registers
When we make a function call we switch to a different register set
Needs a lot of extra registers

When we run out of register sets we start storing the registers in memory

If not we use a call stack in memory.


##### Calling Conventions
We can have caller or callee save registers
We have each save some.
Split the assignment of registers to save.

s0-s2 registers which the callee must preserve if it wants to use them.
t0-t2 registers the caller must preserve if it wants their values to persist over a function call.

Do we always need to put return value on the stack. We can put some return results in a register. We can call the register v0

Parameters can go into a0-a2. 4th parameter goes on stack.

Use the stack sparingly to save memory accesses.

### Registers
- s0-s2 callers "save" registers
- t0-t2 are temporary registers
- a0-a2 are parameter passing registers
- v0 is for return value

- zero always reads 0
- ra is used for saving return address
- at is used for jump target address
- sp is stack pointer

#### Activation Record
Stack frame

- Stack grows toward lower memory addresses
- Decrement then push
- pop, then increment
- Top of stack points to last item placed in it
Never reference past the end of the stack

###### Calling Convention
1. Caller saves any t registers it needs after function call.
2. Caller places 3 parameters into a registers. Everything else goes onto stack.
3. Caller allocates space for addition return values on stack. If it knows its return will not fit into v0.
4. Caller saves previous return address currently in ra
5. Caller executes at, ra
6. Callee stores previous frame pointer then copies contents of stack pointer into frame pointer
7. Callee saves s registers that it plans to use
8. Allocate space for local variables
9. Body of callee runs and leaves return result in v0/in additional return spaces
10. Callee restores s registers from stack
11. Callee Replaces the value in SP with the value from FP to pop the Local Variables and Saved registers off the stack.
12. Caller restores previous return address to ra and pops it off stack???
13. Callee executes JALR to return to caller
14. Caller can get return values and pops it off stack
15. pops off parameters
16. Caller Restores t registers


How stack looks
- Local Vars
- Saves s registers
- ra
- additional return values
- additional parameters
- saved t registers

Recursion does not need anything else
Do need to keep up with frame pointer


Dynamically sized arrays on stack are strange
This can cause stack pointer can change.
This is why we have frame pointer.

###### Differences from LC-3
- Caller must save t registers
- First 3 arguments are passed in registers
- caller must save return address in ra 
- frame pointer points to saved previous frame pointer not the first local variable
- Callee pushed saved s registers before allocating the local variables








