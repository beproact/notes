### Memory Storage
Getting stuff from memory is significantly slower than registers.
We can save memory accesses by saving information in registers.

We can't make it go faster but we can make it go in parallel

###### How to deal with a struct

base + offset

- Elements of a struct are contiguous in memory
- How do we load a.b and a.c into register
	- Lets say &a is already in register r1
	- $R_{2}$ <- memory\[R1+0\]
	- $R_{3}$ <- memory\[R1+4\]

Byte addressable memory so we add 4

ld $r_{i}$,offset($r_{base}$)

ld r2, 0(r1)
"Load the memory at r1 + 0"

ld r3, 4(r1)
"Load the memory at r1+4"

Addressing mode refers to the way the operands are specified in an instruction

char: 8bits = byte
short >= 16 bits = half word
int >= 32 bits = word
long <= 64 bits

ldb(load byte)
ldh(load half-word)
ld or ldw (load word)
ldl (load long-word)

#### Operand Alignment
We generally write addresses write to left.
```c
struct {
	char a;
	char b[3];
}s;
```
####
Dense packing
b\[2] b\[1] b\[0] a



```c
struct {
	char a;
	int b;
}
```
dense packing is ugly here

| b   | b   | b   | a   |
| --- | --- | --- | --- |
|     |     |     | b   |


| wasted | space |     | a   |
| ------ | ----- | --- | --- |
| b      | b     | b   | b   |
Now we only have to do one memory access to get b. We don't have to do anything strange to load b.

RISC is that we should minimize hardware complexity

Hence the need for "natural alignment". Address we store at should generally be a multiple of 4. We don't a type to cross over byte alignments.



#### Accessing Array Operands
```c
int a[100]
```
Just add the offset
 to load a\[8]
ld r8 32(r1)

base+index addressing

r1 =100
r2 = i * 4
ld r8 r2(r1)


#### Endianness
Big endian is how we people normally write numbers. Higher addresses have the least significant bits.
Little endian is dominant today. Lower addresses have the least significant bits.


The difference shows up when taking a “word” apart (in this case, loading 8 bits from a 32-bit integer
0x11223344
ldb  r1, Mem\[104]
Big Endian 🡺 loads 0x11 into r1
Little Endian 🡺 loads 0x44 into r1

### Conditionals
- Evaluate predicate
- Break Sequential flow
	- Need to know where we are
		- PC
	- Need a new instruction for that
	- BEQ r1,r2, offset
		- Branch if r1 == r2
		- PC+PC+offset
		- PC relative addressing mode
- Rejoin control flow
	- unconditional jump
	- we can make an uncondition jump beq r1, r1, offset

#### Switch
Can use a jump table
Address for each case.
indirect addressing mode
