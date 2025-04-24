- [ ] Applications of Telemetry in Medicine
	- Remote Measurement 
	```mermaid
	flowchart LR
	Measurand --> Transducer/sensor --> Signal_Conditioner --> Transmitter --> reciever --> Signal_Conditioner2 --> End_device
	```
	- signal conditioner1 -tranducer output to compatible signal from transmitter
	- transmitter - modulation amplification multiplexing signal conversion for transmission
	- receiver - demodulation amplification reverse signal conversion de multiplexing
	- signal conditioner2 - processes receiver output as needed to drive end device
	- WIRED Telemetry
		- uses pair of copper wires to transmit
		- transmitter has AF/Pulse modulator and amp
	- Digital wired
		- uses A/D converter to process an transmit of telephone lines via modem
	- WIRELESS TELEMETRY
		- transmitter contains RF modulator and amp 
		- connected to antenna
	- Typical Telemetry
		```mermaid
		flowchart LR
		subject --> biopotential --> amp --> processor --> modulator --> antenna
		carrier --> modulator
		subject --> transducer --> amp
		exciter --> transducer
		```


	- applications
		- extended coronary care patient monitoring 
			- each patient has ECG electrodes securely taped to chest
			- which are connected to battery operated transmitter unit containing signal conditioning elements
			- usually housed securely on a belt
			- connected to a channel on ECG patient monitor
		- During Excercise
			- diagnostics for certain abnormalities can only be done under strain aka while moving/running
			- These are also using similar setup to cornoary care patient monitoring systems]
		- Emergency Patient Monitoring
			- in remote areas the ambulances may have systems that transmit data to the hospitals along with two way voice communication 
			- This allows ECGs to be monitored and neccessary preparations made before arrival of patient 
		- Telephone links :- certain ECG units can be coupled with cellphones to provide remote info for the doctor to schedule appointments
		- 
- [ ] Working of PH meter
- [ ] Pacemakers WORKING DIAGRAM
- [ ] Cardiac Defibrillator WORKING DIAGRAM
- [ ] Spectrophotometer WORKING DIAGRAM
- [ ] Dialyzer WORKING DIAGRAM **TYPES**
- [ ] Diathermy significance
- [ ] Single Channel Telemetry System WORKING DIAGRAM
- [ ] Flame Photometer WORKING DIAGRAM
- [ ] PACEMAKER atrio synchronous WORKING DIAGRAM
- [ ] AC defibrillator WORKING DIAGRAM
- [ ] Heart-Lung Machine
- [x] Biotelemetry system
- [ ] OXYMETER blood cell counter