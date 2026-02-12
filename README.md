# 3.-Design-and-Simulation-of-half-wave-rectifier-controlled-by-a-thyristor
## AIM
To design, simulate and analyse a half wave controlled rectifier using one thyristor in MATLAB Simulink.
## APPARATUS REQUIRED
•	MATLAB
## PROCEDURE
1.	Open MATLAB and click on the icon for SIMULINK as shown below
 <img width="522" height="376" alt="image" src="https://github.com/user-attachments/assets/10099b36-8e13-4c8b-836a-053a0059af89" />

Another way is to open is through START icon of MATLAB Start ⇒ Simulink ⇒ Library  browser. 

2.	Click on NEW MODEL or go to FILE ⇒ NEW ⇒ MODEL and a new blank model is created as shown below
 <img width="572" height="382" alt="image" src="https://github.com/user-attachments/assets/50a705b7-b218-45e9-8ecc-852931c3cf65" />

3.	After creating a blank model you need to open the SIMULINK component storeroom/library by going to View ⇒ Library Browser. Select SIMPOWER SYSTEMS then select Power Electronics library and by right clicking on Thyristor and click on add to the model will add the Thyristor in the blank model. Alternatively you can drag the component directly in the model page as shown below
 <img width="940" height="361" alt="image" src="https://github.com/user-attachments/assets/8727c48a-1de5-48e4-b988-8fb57810051f" />

4.	Similarly go to ELECTRICAL SOURCES ⇒ AC Voltage Source and add it to the model. Select Elements and select “SERIES RLC BRANCH” and add it to the model. Simulink do not perform simulation unless and until a measurement block is present in a system. Since we need to measure the input and output voltages and the load current. To add them select Measurement in SIMPOWER SYSTEMS and then add current measurement and voltage measurement blocks to the model. Oscilloscope is not included in SIMPOWER SYSTEMS and is present in the top most block of the left column that is SIMULINK ⇒ Sinks ⇒ Scope. We can join various blocks by clicking on their edges and then drag the wire till the other connection terminal.
5.	Construct the circuit by joining them together in the form as given below
 <img width="940" height="369" alt="image" src="https://github.com/user-attachments/assets/764689de-93f5-4dab-8181-e1dbb78aaaef" />

6.	Now double click the voltage block to set the values of voltage and frequency.
 <img width="349" height="325" alt="image" src="https://github.com/user-attachments/assets/0f991b52-bb8e-44eb-aad6-6014616271c5" />

7.	Double click on Thyristor and you can set various parameters for Thyristor according to the specific data sheet.
8.	Double click on series RLC branch, Select the Branch type as R and set the values for R.
9.	In the Scope menu “>” is shown which can only be connected to the inverse icon “<” in the measurement blocks.
10.	Double click on SCOPE and then click on parameter icon as shown
 <img width="838" height="377" alt="image" src="https://github.com/user-attachments/assets/8a85cb75-cb72-4275-b466-15a925069b7b" />

11.	Make the number of axes as required.
12.	Before simulation also adjust the data history of scope by following
 <img width="363" height="278" alt="image" src="https://github.com/user-attachments/assets/6d9edb83-b273-4d72-852a-77dae5135677" />

13.	Before running the simulation, we have to configure the parameters. Go to Simulation ⇒ Configuration parameters as shown
 <img width="542" height="399" alt="image" src="https://github.com/user-attachments/assets/d2ff10d3-d4ed-47fa-a4a4-a4bd44758389" />

14.	Select the ode23tb (Stiff/TR-BDF2) or ode15s (Stiff/NDS) or any suitable solver as
shown below 
 <img width="566" height="401" alt="image" src="https://github.com/user-attachments/assets/6e638a37-74c5-461e-91b5-bfea3f71e8ee" />

15.	Start the simulation by either clicking on Start Simulation icon as shown in below or
by going to Simulation ⇒ Start
 <img width="770" height="308" alt="image" src="https://github.com/user-attachments/assets/2142a52f-0e16-4984-a4c0-f51fa146713d" />

16.	Double click on scope and observe the graphs.
17.	Left click on any graph and drag to make a rectangle to get the waveforms for a small period of time.
18.	Right click on each graph and select the axes properties and label each graph.
19.	Save the file. ( It should be noted that Simulink do not allow to save files with spaces therefore usually is included in between two words.)
20.	Analyze and record your inference.

## Task
Design, Simulate and analyse single phase half wave rectifier controlled by SCR with the following details 
Vm=100
Frequency = 50Hz
Resistance = 1 ohm
Phase delay or delay angle of Thyristor = 45 degree
After analysing the simulated output,
(i)Draw various simulated waveforms on the graph sheet
(ii) Change the value of resistance to 2 ohm, simulate and draw the current waveform on the graph sheet.
(iii) Change the firing angle to 90 degree, simulate and draw the Output voltage and current waveform on the graph sheet.
(iv)Write your inference.

## Simulation
<img width="1617" height="577" alt="image" src="https://github.com/user-attachments/assets/3deb2a55-7d47-4b42-ad95-4b11a0f42c28" />

## Output
<img width="1897" height="952" alt="image" src="https://github.com/user-attachments/assets/731fe07c-a770-4698-ac0c-87244d9dce33" />

## Result
Thus the experiment was simulated and output was verified succesfully
