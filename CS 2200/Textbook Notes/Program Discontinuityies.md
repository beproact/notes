## 4.3
Interrupts Exceptions and Traps


#### 4 Tricky Things
1. Can happen anywhere during instruction exection
2. Unplanned for
3. When do we tranfer control to the handler
4. We have to return to normal program execution

##### Interrupt Vector Table
Each discontinuity is given a unique number referred to as a vector. Serves as a unique index into the IVT. It is set up at boot time.
Processor uses this table to look up a specific handler address.

###### Traps and Exceptions
Hardware generates this vector internally. We have a new exception/trap register(ETR). When we have an exception or trap we then place the number associated with in the ETR.

1. Architecture defines exceptions and vectors associated. Usually runtime errors
2. OS may define exceptions and traps and specify vectors.
3. OS sets up IVT with addresses of handlers for discontinuities.

### 4.3.1
Modifications to the Finite State machine
