
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
- [x] Cardiovascular System explain DIAGRAM 
- [ ] Electroconduction System of the Heart
- [ ] ECG RECORDING SYSTEM DIAGRAM
- [ ] ECG Lead Configuration
	- ECG machine uses wires with electrode attached to them called leads
	- These leads measure difference in electric potential between
	- they can be bipolar - two points on the body
	- unipolar one point and a virtual zero reference
	- Standard Limb Leads or Bipolar / Eindhoven Leads I II III
		- The standard Limb Leads are used to display a graph of potential difference recorded between two limbs at a time, In these leads , one limb carries the positive electrode and the other limb negative
		- the three electrodes form Einthoven's Equilateral Triangle at Right Arm Left Arm and Left Leg

| LEAD | Positive Electrode | Negative Electrode |
| ---- | ------------------ | ------------------ |
| I    | LA                 | RA                 |
| II   | LL                 | RA                 |
| III  | LL                 | LA                 |
		- The three limbs electrodes form a triangle Eindhoven's Equilateral Triangle
		- Einthoven said that at any point in time of the cardiac cycle the electrical axis of the heart can be represented as a two dimensional vector
		- the sides of triangle represent the individual Lead readings and their algebraic sum of two is equal to the third and their vector sum is zero
- [x] ECG electro cardiography
- [ ] analysis of ECG signal
- [ ] Measurement of blood pressure direct indirect relative
- [ ] oscillometric ultrasonic noninvasive pressure measurement
- [ ] Ultrasonic Blood flow meters
- [ ] systole and diastole
- [x] Einthoven's triangle
- [ ] korotkoff sounds
- [ ] doppler effect significance in blood parameter measurement
- [ ] explain auscultatory method for measurement of blood pressure DIAGRAM
- [ ] unipolar limb lead configuration with DIAGRAM