
- [ ] 10-20 electrode scheme DIAGRAM
	- 21 electrodes separation of 10%/20% of the distance between nasion and inion between each electrode
	- Fp 1/2 - frontal polar 10% from nasion vertically as well as horizontally
	- F 4/8 - 20% front Fp2 vertically and 10 and 30% respectively from central line Fz to the right
	- F 3/7 - 20% from Fp1 vertically and 10 and 30% respectively from Fz to the left
	- C Central
	- P parietal
	- T Temporal - halfway 
	- O Occipital - 10% from inion
	- ODD numbers left
	- even numbers right hemisphere
	- z for central line electrodes
	- A- reference/earlobes
- [ ] EEG Recording Modes, System DIAGRAM
	```mermaid
	flowchart LR
	electrodes --> jackbox --> electrode_montage_selector --> Amplifiers/Filters_Hi-pass/Low-pass/notch_sensistitvity --> Analog_to_digital_converter --> oscilloscope
	Analog_to_digital_converter --> Computer -->EEG
	Amplifiers/Filters_Hi-pass/Low-pass/notch_sensistitvity --> WriterUnit --> Chart_drive --> EEG
	WriterUnit --> ink-writingoscillograph
	```
	- Montages refer to pattern of electrodes on the head and channels they are connected to
		- reference electrodes are placed on non active region forehead/earlobe
		- 10/20system
		- 21 electrodes
		- 10 and 20% of the distance between nasion and inion seperation between the electrodes
	- Electrode Montage Selector
		-  large panel to allow user to select electrode pairs
		- each channel is input from one electrode minus input from another
	- Preamp
		- every channel has individual multistage, ac coupled,very sensitive amplifier with differential input and adjustable gain in a wide range
		- high gain low noise since signals are low amplitude
		- HIGH CMRR 
		- no drift
	- Sensitivity control
		- one adjusts sensitivity of recording pen
		- a continuously variable one to equalize the sensitivity of all channels
		- one with known step values for each individual channel gain control
	- Filters - noise removal
	- Writing Part 
		- The writing part of an EEG machine is usually of the ink type direct writing recorder
		- The best type of pen motors used in an EEG have a frequency response of 90Hz
		- some have 45Hz inkjet system has a response of 1000Hz
	- Paper Drive - This is provided by a synchronous motor speed 15,30,60mm/s
- [ ] body plethysmograph DIAGRAM
- [ ] Electrical stimulation of muscle and nerve
- [ ] Physiology of Respiratory System DIAGRAM
- [ ] Working Principle of Spirometer DIAGRAM
- [ ] physiology of Human Nervous system DIAGRAM
- [ ] Placement of EEG electrode DIAGRAM
- [x] Brain Waves and when they occur
- [ ] **Respiratory Parameters DIAGRAM** AND MEASUREMENT PHYSIOLOGY GAS EXCHANGE
- [ ] Neuron Membrane Potential DIAGRAM
- [ ] Functional Electrical stimulation PRINCIPLE and APPLICATION
- [ ] EMG analysis acquisition of signal
	- technique for evaluating and recording the action potential of muscles
	- 50 $\mu$V to 30 mV
	- Surface electrodes:-
		- used to monitor electrical activity of muscles
		- gets general activity
	- Needle electrodes:- 
		- to monitor electrical activity few muscle fibers
		- needle is inserted through the skin
	```mermaid 
	flowchart LR
	Body_Part --> EMG_Electrode --> Bio-Electric_amplifier --> EMG_Recorder
	Bio-Electric_amplifier --> AF_Amplifier
	Bio-Electric_amplifier --> Oscilloscope
	```
	- EMG electrode :- electrode for EMG can be surface or needle
	- bio electric amp
		- high gain
		- high cmrr
		- amplifies EMG signal from few micro to milli volts
	- AF amp:- normal muscles produce electric sound when needles being inserted damaged muscles produce different sound. AF amp distinguishes these early on
	- Oscilloscope to visualize the EMG. DSO can store it
	- EMG Recorder:- photographic recording on light sensitive paper
- [ ] EMG myoelectric Control System
- [ ] Analysis of EEG signal
- [ ] evoked potential



















[[BIOMED]]