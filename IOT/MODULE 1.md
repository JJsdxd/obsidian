- [ ] IOT
	- describes physical objects(things) with sensors, processing ability, software and other technologies that connect and exchange data over the internet or other communication networks
- [ ] Characteristics of IOT
	1. Dynamic & Self Adapting
		1. IOT devices should have the ability to make dynamic changes based on available context from user/sensed environment
		2. eg :- surveillance cameras changing modes based on day and night by time/light sensing
		3. eg :- lower to higher resolution modes if any motion is detected to save on storage as well retaining correcting recordings of relevant times
	2. Self-Configuring
		1. The ability of an IOT device to setup to IOT infrastructure provided networking and fetch software upgrades with limited/zero user intervention
		2. This ability allows a large number of devices to work together to provide functionalities
	3. inter operable Communication Protocols
		1. support number of inter operable communication protocols to communicate with other devices as well as IOT infrastructure
	4. Unique identity/Uniquely Identifiable
		1. Each device should have its own unique identifier/unique identity (IP address)
		2. IOT interfaces allow users to
			1. query devices
			2. monitor their status
			3. remotely control
	5. Integrated into Information Network
		1. IOT devices are usually integrated into a information network which allows them to communicate with other devices and systems for exchanging data.
		2. This integration allows the IOT devices to become smarter using collective intelligence
		3. allows for larger data to be aggregated and analysed to predict weather etc..
		4. weather monitoring nodes communicating is an example
- [ ] IOT Enabling Technologies
	- wireless sensor networks
		- is a distributed devices with sensors tasked with monitoring the enviornmental and physical conditions
		- consists of number of end nodes routers and coordinators
		- each end node has several sensors attached to them
		- end nodes can also act as routers
		- Coordinator collects data and acts as gateway to internet
			- weather monitoring
			- smartgrid
			- indoor air quality monitoring systems
	- cloud computing
		- Cloud computing is a transformative computing paradigm 
		- delivering services and appllications through the internet
		- resource provision is automated
		- provides computing networking and storage devices
		- standard a
	- big data analytics
	- embedded systems
	- communication protocols
	- 
- [ ] Physical Design of IOT
	- The Things in IOT usually refers to devices that are uniquely identifiable can perform remote sensing/actuating/monitoring capabilities
	- IOT device can
		- exchange data with other connected devices and applications
		- collect data from other devices and process the data locally
		- Send the data to centralized servers or cloud based application back-ends for processing the data
		- Perform some tasks locally and other tasks within the IOT Infrastructure based on temporal and space constraints
	- IOT device can contain several interfaces
		- I/O for sensors
		- Interfaces for Internet Connectivity
		- Memory and Storage Interfaces
		- Audio/Video Interfaces
	- Connectivity 
		- USB HOST
		- RJ45/INTERNET
	- Processor
		- CPU
	- Audio/video interfaces
		- HDMI
		- 3.5mm
		- RCA video
	- I/O interfaces
		- UART 
		- SPI
		- I2C
		- CAN
	- Storage Interfaces
		- SD
		- MMC
		- SDIO
	- Graphics - GPU
	- Memory Interfaces
		- NAND/NOR
		- DDR1/DDR2/DDR3
- [ ] Levels of IOT - Deployment Templates
- [ ] IOT Functional Block
	- logical design of an IOT refers to an abstract representation of the entities and processes without going into the low-level specifics of the implementation
	- **Application** TOP Center-
		- IOT application provides an interface that allows user to control and monitor various aspects of the system
		- Application also allow users to view the system status and view or analyze the processed data
	- **Management** LEFT-
		- functions to govern the system
	- **services** center top-
		- an IOT system uses various types of IOT services for data monitoring, data publishing, device discovery etc..
	- **Communications** center bot-
		- Communication block handles the communication for the IOT System using communication protocols
	- **Security** Right-
		- secures IOT system by providing functions like authorization,authenication, message and content integrity, data security
	- **Device** bot-
		- A system that comprises of sensing actuation monitoring and control functions
- [ ] IOT communication models
	- **Request-Response**-
		- Client sends Requests to server and Server responds to requests
		- Server upon receiving request decides how to respond fetches data gets resource representations , prepares the response and then sends the response to the client 
		- Each request-response pair is independent of other
	```mermaid
	flowchart LR
	Client -->|Request| Server <-->|data fetching|Resources
	Server -->|Response|Client
	```
	- **Publish Subscribe**-
		- This involves Publishers brokers and consumers
		- Publishers are source of data
		- publishers send the data to the topics which are managed by the broker 
		- publishers are not aware of consumers
		- consumers subscribe to topics managed by the broker
			- Once broker receives data for a topic from the publisher, it sends the data to all the subscribed consumers
	- **push-pull**-
		- Push-pull is a communication model in which data is pushed into queues by data producers and the consumers pull data as necessary
		- Producers are unaware of consumers
		- Queues act as a buffer which helps in situations when there is a mismatch between rate at which producers push data and the rate at which consumers pull data
		```mermaid
		flowchart LR
		Producer --> Queue1 -->|message pull| consumer1
		Producer -->|message pull| Queue2 --> consumer2
		```
	- Exclusive Pair
		- Exclusive Pair is a bi-directional, Fully Duplex communication model that uses a persistent connection between the client and server
		- Once setup the connection is only closed upon client request
		- messages can be sent to and fro after setup
		- Server is aware of all open connections
		- client is aware of the server which it connects to
		```mermaid
		flowchart LR
		Client -->|Request to setup Connection|Server
		Server -->|Response accepting connection request|Client
		
		Client -->|message to server from client|Server
		
	
		
		Server -->|Message from server to client|Client
		
		Client -->|Request to close Connection|Server
		Server -->|Connection Close Response|Client	
		```
	-
- [x] Architectural View
- [x] Logical Design









[[IOT]]