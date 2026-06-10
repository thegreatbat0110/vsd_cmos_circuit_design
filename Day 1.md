-------------------------------------------------------------------------------------------------
D1SK1
------
Introduction
--------------
Gates are made of PMOS n NMOS transistors.
W/L ratio decides value of current which in turn descirbes waveform shape.
SPICE simulation is a widely used software process that mathematically predicts the behavior of electronic circuits before they are physically built. It uses mathematical models and laws (like Ohm's Law and Kirchhoff's laws) to calculate voltage, current, and signal integrity across a circuit's components.
Spice Simulation - used in clock tree synth , pd etc
Input slew (transition time) and output load (capacitance) are the two critical variables used to calculate how fast a logic gate propagates a signal. Together, they determine the circuit's delay and overall power consumption
<img width="558" height="315" alt="image" src="https://github.com/user-attachments/assets/d8d4aaaf-8748-432c-a966-2ba69714a500" />
In VLSI, delay is the finite time required for an electrical signal to travel through a circuit. It directly limits chip performance (clock speed) and is divided into cell delay (time taken by logic gates to switch) and interconnect/net delay (time taken for signals to travel across wires).
Delay comes from - 

NMOS
-----


