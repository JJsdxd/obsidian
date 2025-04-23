
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
- [x] Cardiovascular System explain DIAGRAM 
- [x] Electroconduction System of the Heart
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
	- Augmented limb leads
		- avR right arm, aVL Left arm, aVF LEFT FOOT
		- each lead is recorded in reference to the other two electrodes conjoined
		- the other leads are connected to positive and are called averaging electrodes and the resistances connected are called averaging resistances
	-Precordial Leads
		-second type of unipolar leads uses 6
		- V1-4th intercostal space right sternal margin
		- V2 - 4th intercostal space left sternal margin
		- V3 - midway between V2 and V4
		- V4- fifth intercoastal space at mid clavicular line
		- V5 - same level as V4 at anteriror axilliary line
		- V6 - " at mid axialliary line
- [x] ECG electro cardiography
- [ ] analysis of ECG signal
	- its quasi periodical , rhythmically repeating signal
	- P- atrial contraction
	-  R marks ending of atrial contraction and start of ventricular contraction
	- QRS -repolarization of atria and depolarization of ventricles
	- T - repolarization of ventricles
	- PR - time taken from atria to AV node
	- QRS - time taken from intro ventricular system and then to ventricular contraction
- [x] Einthoven's triangle
- [x] unipolar limb lead configuration with DIAGRAM
- [ ] Measurement of blood pressure direct indirect relative
	- Indirect
		- simple equipment
		- cannot measure when pressure very low
		- Auscultory:-
			- uses aneroid sphygometer with a stethescope
			- a cuff is placed on your arm and inflated with a pump till circulation is cut off
			- slowly deflates the cuff while listening for blood sounds using stethescope
			- first sound of blood refers to systolic pressure kokorotkoff sounds
			- once it fades is the diastole
			- pressure cuff, mercury manometer, valve, air pump on brachial artery, listen on radial artery branching point
		- oscillometric 
			- occuluding cuff deflating results in artery walls vibrating due to turbulent blood flow through partially occluded arteries which can be detected via the transducer monitoring cuff pressure, as pressure continues to decrese the vibrations increase to a maximum point and then 
- [ ] oscillometric ultrasonic noninvasive pressure measurement
- [ ] Ultrasonic Blood flow meters
- [ ] systole and diastole
	- systole :- highest pressure on the vessel walls when the heart is beating and pumping blood through the body
	- diastole:- the lowest pressure on walls when heart is resting/in between beats
- [ ] korotkoff sounds
- [ ] doppler effect significance in blood parameter measurement
- [ ] explain auscultatory method for measurement of blood pressure DIAGRAM
- [ ] Electromagnetic Blood Flow meter DIAGRAM and WORKING
	- measure instantaneous pulsatile blood flow 
	- based on electromagnetic induction
	- voltage induced in a conductor in a moving magnetic field is proportional to the velocity of conductor
	- blood is the moving conductor
	- permanent /electro magnet around the blood vessel 
	- magnetic field perpendicular to the flow of blood
	- the potential build up in the blood is measured by the sensing elements 
	- magnitude of voltage picked up is directly proportional to velocity of blood
	- e = CHVd Q=Va   e = CHdQ/a
	- Types
		- sine wave:-  gated amplifier used to remove transformer voltage 
		- voltage is 90$\degree$ out of phase with input sine wave
