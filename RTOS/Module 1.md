- [ ] Functions of OS
	- PROCESS MANAGEMENT
	- JOB ACCOUNTING
	- MEMORY MANAGEMENT
	- FILE MANAGEMENT
	- DEVICE MANAGEMENT
	- SECURITY
	- SECONDARY STORAGE MANAGEMENT
	- PROCESS MANAGEMENT
	- NETWORKING
	- CORDINATION BETWEEN OTHER SOFTWARE AND USERS
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
	- is a collection of system programmes providing user/applications with a means to access the resources in a computer
	- Types of OS
		- Batch OS
			- No direct access to the computer
			- every user works on a device like a punch card which are then handed over to a computer operator
			- similar need programmes are grouped together to  be more efficient and increase speed of processing
				- allows multiple user at the same time
				- lowers net time taken to run all the programmes
				- If a job fails other jobs will have to wait for an unknown amount of time
				- Batch Systems are Expensive
				- Hard to Fix bugs
				- 
		- Multi_Processor OS
			- When more than one processor is present multi processor OS can be used to take advantage of this increased resource availability
			- This can significantly cut down on the amount of time needed to execute programmes 
			- by making use of parallel execution of multiple programmes
				- Allows multitasking like in modern systems
				- Games, Scientific Calculations, Financial computing etc..
				- More Expensive due to the higher number of CPU and memory units required
		- Multiprogramming OS
			- Single Processor runs multiple Programmes at the same time
			- when a programme is waiting for I/O the processor has other programmes ready to use the CPU
			- multiple jobs share CPU time
			- The jobs are not executed in parallel/at the same time
				- Reduced Reaction time
				- ability to perform multiple tasks within same programme at once
				- multiple people's need can be satisfied at once
				- short term tasks get executed faster
				- Short term projects could receive great speed increases
				- increased CPU and other resource utilisation
				- -
				- Extremely intricate and increased complexity
				- Processor Scheduling is Essential
				- Increased need for memory management
				- 
		- Distributed OS
		- Time Sharing OS
		- Real Time OS
- [ ] OS as Resource Manager
	- OS controls the movement, storage and processing of data
	- OS functions as an ordinary computer software
	- OS relinquishes controls or regains control Depending on processor
	- This Control mechanism is an internal mechanism
	- Resources under control of the OS
		- Main memory
		- I/O devices and files
		- processor
	- Main memory
		- a portion of the OS(kernel) resides in the main memory
		- Kernel contain
			- Frequently used functions
			- Portions of OS which are currently in use
		- Main memory = kernel + user programs + data
		- Main memory allocation is done by OS and by a memory management hardware in the processor
	- I/O and FILES
		- Decides and allocates when an I/O can be used by a program in execution
		- Controlled access of files
	- Processor Control
		- Determines how much time and when a program/process gets to access processor
	```mermaid 
	flowchart LR
	subgraph kernel
	I/O_Controller
	subgraph Memory
	Operating_System
	Programs_&_Data
	end
	Processor
	end
	I/O_devices <--> I/O_Controller
	I/O_Controller <--> Storage
	```
- [ ] microkernel
- [ ] exokernel
- [ ] OS as User/Computer Interface
	- Program Development:-  Editors/Debuggers assist programmer in writing and debugging application programs These are provided in the application program development tool
	- Program Execution :- These are load-program run-program execute-program 
	- Access to I/O Devices :- a controlled and uniform means to access I/O device which is hidden from the end user
	- Controlled Access to Files :- OS provides controlled access based on it's understanding of the I/O structure and for security of user in multiuser systems
	- System Access :- Provides access to System as a whole and to specific System Resources . To resolve conflicts for Resource Retention
	- Error-Detection :- An OS must be constantly aware of possible errors
		- These may occur in CPU, I/O, memory etc..
		- for each type of error OS should take the appropriate action to ensure correct and consistent computing
		- Debugging facilities can greatly enhance User's experience and programmers ability to utilise the system efficiently
	- Accounting :- keeping track of when how and which user used what resources in a computer

- [ ] Process Control Block
- [ ] Monolithic
- [ ] Microkernel
- [ ] Process State Diagram

- [ ] kernel
- [ ] Operations on processes







[[RTOS]]