- [ ] Functions of OS
- [ ] microkernel
- [ ] exokernel
- [ ] OS as Resource Manager
- [ ] Process Control Block
- [ ] Monolithic
- [ ] Microkernel
- [ ] Process State Diagram
- [ ] Computer System
	- Can be divided into 4 parts
	- Hardware 
		- provide basic computing resources I/O, CPU, memory
	- Operating System
		- controls and coordinates the use of hardware among various users and applications
	- Application Programs
		- Software that uses computer hardware to solve computing problems often specialized
		- word processors, web browers etc
	- Users - humans  machines other computers, etc
	```mermaid
	flowchart LR
	User_1 --> compiler
	User_2 --> assembler
	User_3 --> text-editor
	User_n --> database

	compiler --> Operating_System
	assembler --> Operating_System
	text-editor --> Operating_System
	database --> Operating_System

	Operating_System --> Computer_Hardware
	```
- [ ] Objectives of OS
	- a Program that acts as an intermediary/interface between user and the computer hardware
	- execute user programs and make solving user problems easier
	- make computer system convenient to use
	- Use the computer Hardware in an efficient manner
- [ ] kernel
- [ ] Operations on processes







[[RTOS]]