- [ ] Functions of OS
- [ ] microkernel
- [ ] exokernel
- [ ] OS as User/Computer Interface
- [ ] OS as Resource Manager
	- OS controls the movement, storage and processing of data
	- OS functions as an ordinary computer software
	- OS relinquishes controls or regains control Depending on processor
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
	```mermaid
	flowchart 
	End_User --> Application_Programs
	Application_Programs --> Utilities
	Programmer --> Utilities
	Programmer --> Operating_System
	Utilities --> Operating_System

	Operating_System_Designer --> Computer_Hardware
	Operating_System --> Computer_Hardware
	```
- [ ] Objectives of OS
	- a Program that acts as an intermediary/interface between user/userprogrammes and the computer hardware
	- execute user programs and make solving user problems easier
	- **CONVENIENCE** - make computer system convenient to use
	- **EFFICIENCY** -Use the computer Hardware in an efficient manner
	- **ABILITY TO EVOLVE** - to hide details of hardware resources from the user
- [ ] OS
	- Layer of Software built with the purpose of providing User Programs with a simple interface to the computer Hardware
- [ ] kernel
- [ ] Operations on processes







[[RTOS]]