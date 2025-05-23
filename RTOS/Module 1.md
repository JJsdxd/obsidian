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
				- Managing everything is a difficult task
		- Distributed OS
			- Allows the OS to be run on multiple devices at the same time
			- used to spread data and applications
			- used in computer networks to coordinate Their Hardware and Software resources
			- the users may be geographically separated
			- multiple computers share a single data link
			- Each system has its own separate computing power and storage which is not shared
			- These systems may share discs, networking, Hardware, Software nodes, CPU, Network Interfaces etc..
			- More people can access information
			- +
				- These Shared Resources allow for increased speed and efficiency
				- sharing of Resources makes the system cheaper
				- The system allows each system to work on their
				- a single failure won't take down the whole system
				- Computers can be easily added to this system
				- -
					- high setup cost
					- Server failure will be critical
		- Time Sharing OS
			- Invented as an alternative to multiprogramming batch os
			- multiple user simultaneously use the same hardware through different terminals 
			- The OS interleaves the execution of Each user using by providing Short Bursts or Quantum of Computation
			- Minimizes Response Time
			- Commands in Terminal
			- Allows numerous concurrent user through a shared User Interface
			- Prevalent in businesses and such with high Personnel count
			- Enables access to same files/applications to multiple concurrent users
			- +
				- Speedy Response times
				- User Friendly 
				- reduces CPU idle time
				- each task has set duration of time
			- -
				- increased resource utilisation
				- High specification hardware required
				- Security and Integrity of programmes is a concern
				- dependability is a concern
		- Real Time OS
			- This OS is employed when there is a need for the system to process and gather data in a fixed amount of time
			- Usually when data is to be analyzed in Real time
			- There are two types
			- Hard Real time :- in these systems even small delays are not tolerated as these may be system critical 
			- Soft-Real Time :- Here these systems allow for small delays without losing functionality
			- These are commonly Employed in Traffic Control/Medical Systems
				- +
				- Resources and Technology are utilised to their full extent
				- These Systems are nearly error Free
				- -
				- Uses very complicated Algorithms
				- Limited Duties can be performed
				- Increased System Resources for OS
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
- [ ] Monolithic
	- The entire operating system operates in kernel space
	- Simple Operating System where memory, file, device and process management are all done by the kernel
	- These components are all present inside the Kernel
	- This has three major layers
	- Application Layer:-
	- Monolithic Kernel layer
	- Hardware Layer:-
	- Every application in this Operating System has it's own address space as a result the applications are safer
	- kernel has file system, memory manager and CPU scheduler
		- +
		- is faster due to the memory management, file management and process scheduling being implemented in the same address space
		- it has simple structure which is easy to understand
		- all the components have the ability to interact directly with each other indirectly via the kernel
		- works better for smaller tasks as it may handle limited resources
		- -
		- User programs uses same address space as kernel a bug may take down the whole system
		- not easy to port code written in monolithic
		- difficult to add/remove features
		- all the code must be modified and recompiled to do the same
- [ ] kernel
	- The kernel is the Core of the Operating System
	- It is a program that is at the Core of a Computer
	- This is always present in the system memory
	- This facilitates interaction between hardware and software components
	- This is the medium with which the OS controls the hardware components
	- Functions
		- Process Scheduling
			- The kernel provides a part of time for each process to access the processor 
			- After one finishes execution the kernel starts another
		- Resource Allocation
			- kernel has control of CPU, memory, peripheral Devices etc.
			- it acts as the link between processes and resources
			- allocates memory to processes
			- When a Process requires access to any peripheral device/hardware component the kernel allocates the component to it
		- Device Management
			- The kernel is also in charge of managing all peripheral and storage devices connected to the system  as well as controlling the exchange of data between these
			- The information is received from the system and is transferred to the various devices via the kernel
		- Interrupt Handling
			- When a process runs it can be interrupted by a higher priority task to be executed urgently
			- The kernel is responsible for promptly storing the state of the current process and handing over control to the new process
			- The kernel also handles System Calls, which are basically software interrupts
		- Memory management
			- Kernel is responsible for allocation as well release of memory
			- Each process requires memory for its execution
			- after execution this memory should released and reallocated
		- Process Management
			- The kernel is incharge of creation execution and termination of process in a system
			- For the system to execute any task the kernel has to create and manage the processes
- [ ] microkernel
	- minimized kernel size and functionality
	- process management and I/O
	- modularity
	- MicroC/OS
	- abstract
- [ ] exokernel
	- programs can communicate directly with system hardware
	- +
		- ease of development
		- increased performance
		- more efficient and intelligent use of hardware by applications
	- -
		- high complexity
		- Less consistent
	- minimal interface to hardware and relies on libraries for resource management
	- low abstraction


- [ ] Process Control Block
	- Process is a computational unit
	- The execution of a program is known as process/task
	- Each process is under the control of the OS
	- Process :- is sequentially executable program(codes)
	- State control by an OS
	- The state of a process is represented by the information of process state
	- Process runs on scheduling by OS. Process runs Instructions and continuous change takes place as the PC changes
	- Process Image is the collection of program, data and PCB together
	- Process identification, Process state information, Process control information is contained in PCB
	```mermaid 
	block-beta
	columns 1
	Process ID
	Priority
	Process State
	PSR
	Registers
	Event_Information
	Memory_Allocation
	Resources_Held
	PCB_Pointer
	```
	- Process Identification
		- numeric process identifier Process ID (pid)
		- identifier of the parent (ppid)
		- user identifier(uid)
	- Process State Information
		- User visible registers
		- Control and status registers(PC, IR, PSW, interrupt related bits, execution mode)
		- stack pointers
	- Process Control information
		- Scheduling and state information
			- process state
			- priority
			- scheduling
			- awaited event
		- Data Structuring
			- pointers to other PCB (parent/child/same queue)
		- interprocess communication Various flags, signals, messages may also be part of PCB
		- Process privileges
		- memory management
		- resource ownership
	- PCB is very protected
	- 
- [ ] Microkernel
- [ ] Layered OS
	- OS with separate layers for handling user and application software
	- A layered operating system that has divided into multiple layers
	- each layer with a fixed task assigned to it
	- lower layers core system software
	- higher layers deal with application software
	```mermaid 
	flowchart 
	User_Programs --> I/O_buffer --> Process_Management --> Memory_Management --> Scheduling --> Hardware
	```
	- **Hardware** is the lowest layer, it is where the hardware devices are handled 
	- **CPU Scheduling** It manages Scheduling tasks and schedules the processes for CPU
	- **Memory Management** It manages the memory . It moves processes from disk to the primary memory for execution and returns the executed programs to disk
	- **Process Management** It handles the processes, and it also assigns the CPU to execute processes
	- **Input-Output Buffer** It allows the users to interface with the system and controls IO device Buffers and ensure that IO devices work properly
	- **User Programs** It is associated with the user programs like word processor, browser. All the User Programs are handled in this layer
	- +
		- Easy debugging Discrete layers allow the debugging that needs to be done to be limited to the single layer where the error is found
		- Modularity Each layer only performs it's stipulated task 
		- Abstraction Each layer is contained and functions and implementations of the other layer are abstract to it
		- Easy Update a modification of one layer does not require any modification in the remaining layers
	- -ve
		- Complex The layer layout makes the design much more complex as the means of access needs to be robustly defined
		- Slower in Execution  When one layer wishes to interact with another, It sends a request that must traverse all layers between the two layers to be fullfilled increasing layer count may make the design inefficient

- [ ] Process State Diagram
	- new The process is being created
	- running Process that are currently being executed
	- waiting/Blocked  The process is waiting for some event to occur
	- ready  The process waiting to be assigned to a processor
	- Terminated/EXIT The process has finished execution
	```mermaid
	flowchart LR
	new -->|admitted| ready --> |scheduler dispatch| running --> |exit| Terminated/EXIT
	running -->|I/O or event wait| waiting/Blocked -->|I/O Event completion| ready 
	running -->|interrupt| ready
	```

	- Suspended state
		- when no process in memory is in ready state os moves blocked process into suspend queue 
		- when suspended process is ready to run it moves into ready_suspend queue
		- two new states are Ready_suspend and Blocked_suspend
		- Ready_suspend: 
			- process is in secondary memory but is ready for execution as soon as loaded into main memory
		- Blocked_suspend: 
			- The process is in the secondary memory and awaiting event
	```mermaid
	flowchart LR
	NEW -->|admit|Ready -->|Dispatch|Running --> |Release|EXIT
	Running -->|Event Wait|BLOCKED -->|Suspend|Blocked_Suspend -->|Event Occurs|Ready_Suspend -->|Activate|Ready
	Ready -->|Suspend|Ready_Suspend
	Blocked_Suspend -->|Activate|BLOCKED -->|Event Occurs|Ready
	Running -->|Time_OUT|Ready
	```
- [x] Operations on processes







[[RTOS]]