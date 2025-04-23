
- [ ] **ECG WORKING DIAGRAM**
	- Lead Selector Switch:- potentials picked up by the array of leads and transported to lead selector switch where the signals are selected in pairs based on lead program
	- **PreAmplifier**:-
		- The signal from lead selector is amplified in preparation for future processing 
		- usually a 3/4 stage unbalanced output differential amplifier
	- **PowerAmplifier**:-
		- it is a push pull differential amplifier.
		- Single ended output from preamp and an input from frequency selective network is taken as inputs
		- Output is single ended
		- output fed to pen motor
		- Frequency Selective circuit is an RC circuit to provide damping for pen
	- Auxiliary circuits
		- produces 1mV calibration signal and blocking of PREAMP during lead changes it also controls the X axis movement of the chart via chart driver moter

	```mermaid
	flowchart LR
	LEADselector --> PreAmp --> PowerAmp --> BridgeO/Pcircuit --> PenMotor
	AuxilliaryCircuits --> ChartTransportMotor
	AuxilliaryCircuits --> PreAmp
	BridgeO/Pcircuit --> FrequencySelectiveFeedbackNetwork --> PowerAmp
	```
- [ ] Electromagnetic Blood Flow meter DIAGRAM and WORKING
- [ ] Cardiovascular System explain DIAGRAM 
- [ ] Electroconduction System of the Heart
- [ ] ECG RECORDING SYSTEM DIAGRAM
- [ ] ECG Lead Configuration
- [ ] ECG electro cardiography
- [ ] analysis of ECG signal
- [ ] Measurement of blood pressure direct indirect relative
- [ ] oscillometric ultrasonic noninvasive pressure measurement
- [ ] Ultrasonic Blood flow meters
- [ ] systole and diastole
- [ ] Einthoven's triangle
- [ ] korotkoff sounds
- [ ] doppler effect significance in blood parameter measurement
- [ ] explain auscultatory method for measurement of blood pressure DIAGRAM
- [ ] unipolar limb lead configuration with DIAGRAM