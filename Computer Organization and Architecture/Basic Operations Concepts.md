
## **Assembly Language**
==ADD==

> Add LOCA, R0
	> add-> opcode
	> LOCA-> Op1
	> R0-> Op2
- Adds LOCA with R0 register and the result is stored in R0
	- Steps
	1. Instruction to fetch(from memory to CPU)
	2. Operand at LOAC is fetched  > 
	3. Fetched operands is added with R0
	4. Resulting in sum is stored in R0

==Load==

> ADD LOCA, R0
> LOAD R0

----------


![[Pasted image 20220121122005.png]]

- MAR (Memory address register)
- MDR(Memory data register)
- Control(control R/W)
- PC(Program counter)( address of next instruction)
- IR( Current Instructor)

---
## **Bus Structure**

> grp of lines servers as a connection path for several devices.
	>lines of address->address bus
	>data-> data bus
	>control signal->control bus
	
 * ***Address bus size will control the size of memory***
 * 