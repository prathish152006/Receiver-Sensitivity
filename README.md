# Receiver-Sensitivity
Objective: 
Determine the sensitivity of a PIN photodiode based optical receiver by determining the 
minimum received power necessary to achieve a given Q factor. Compare the results of 
simulation with the results of an analytic approach.  
Theory: 
If we include only the effect of thermal noise, the sensitivity of a PIN photodiode-based 
receiver is 
= 
Q
S T
σ
R
where 
• S = sensitivity (W) 
• Q = desired Q factor (related to the desired bit error rate or BER) 
• R = photodiode responsivity (A/W) 
• σT = rms thermal noise current (A) 
The rms thermal noise current σT is given by 
σ 
2
T 
=
ST
where 
B
• ST = thermal noise spectral density (A2/Hz) 
• B = receiver bandwidth (Hz) 
Calculations: 
The table below lists the receiver specifications: 
Operating bit rate 
Bandwidth 
2.5 Gb/s 
1.65 x bit rate 
Thermal noise spectral density X.Y x 10-22 A2/Hz
Desired Q factor 
PIN photodiode responsivity 
6 
1 A/W 
X and Y are the last two digits of your student ID number. For example, if your ID 
number ends with 43, then us ST = 4.3 x 10-22. Determine the receiver sensitivity using 
the formulas given above.  
Layout: 
The layout consists of: 
1. CW laser source 
2. Modulator with a non-return to zero modulator 
3. Optical attenuator 
4. PIN photodiode with an electrical filter 
The PIN photodiode has the responsivity left as its default value, 1 A/W. The dark 
current is set to 0. The ASE noise parameter is turned off.  The thermal noise parameter is 
available for you to edit. 
Power meters have been placed at the output of the modulator and after the attenuator to 
allow you to determine the optical power at the output of the transmitter and the input to 
the receiver. 
Simulation: 
Adjust the output power to obtain a transmission output power 0dBm. Set the attenuator 
to 20dB. Run the simulation.  Adjust the attenuator until the Q factor is 6.00±0.05.  
Report: 
• A neat, well-presented summary of your pre-lab calculations (attach any hand
written calculations). 
• Screen shots or other displays of the results of your simulation including power 
readings BER analyzer display (including eye diagram). 
• Discussion of any differences between the calculation and the simulation results.
