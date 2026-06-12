-------------------------------------------------------------------------------------------------
D1SK1
------
Introduction
--------------
Gates are made of PMOS n NMOS transistors.

W/L ratio decides value of current which in turn descirbes waveform shape.

SPICE simulation is a widely used software process that mathematically predicts the behavior of electronic circuits before they are physically built. It uses mathematical models and laws (like Ohm's Law and Kirchhoff's laws) to calculate voltage, current, and signal integrity across a circuit's components. It's used in clock tree synth , pd etc.

Input slew (transition time) and output load (capacitance) are the two critical variables used to calculate how fast a logic gate propagates a signal. Together, they determine the circuit's delay and overall power consumption

<img width="558" height="315" alt="image" src="https://github.com/user-attachments/assets/d8d4aaaf-8748-432c-a966-2ba69714a500" />

In VLSI, delay is the finite time required for an electrical signal to travel through a circuit. It directly limits chip performance (clock speed) and is divided into cell delay (time taken by logic gates to switch) and interconnect/net delay (time taken for signals to travel across wires).


NMOS
-----

<img width="677" height="287" alt="image" src="https://github.com/user-attachments/assets/844826c5-66c1-472b-af24-e2cd9a183520" />

A MOSFET is a single electronic component (a tiny voltage-controlled switch). 

CMOS is a circuit design technology that teams up two different types of MOSFETs (one to pull power up, and one to push power down) to do complex logic and run microprocessors with almost zero wasted energy.

<img width="571" height="224" alt="image" src="https://github.com/user-attachments/assets/53c052a6-4ddd-4529-bc56-8990b768d4b9" />

When we give +ve charge other sides =ve charge is repelled leaving negative charge.

Upon increaing gate voltage  - depletion region width increases.

Strong / surface inversion After a while teh a small portion p substaret will be converted to n type mterial

After this there isi ono increase in depletion region width but increase in channel width

Thresold Voltage - v at which strong ncersion occurs

<img width="520" height="271" alt="image" src="https://github.com/user-attachments/assets/e781ba37-523a-4a9c-acb1-0f51a801a1c3" />

Body terminal  -



-------------------------------------------------------
D1SK2

Spice simulations -> delays.

Feed models to spice engine.

Some constants - spice model parameters (circled) given to SPICE. They need not be derived. Special file exists.

<img width="212" height="231" alt="image" src="https://github.com/user-attachments/assets/033c3cb4-2079-4135-bd39-bbea4b40edca" />

Spice model parameters + netlist -> SPICE Software -> graph

<img width="577" height="226" alt="image" src="https://github.com/user-attachments/assets/fd3e7042-c9ed-441f-8a19-c1ba566dec3a" />

Spice netlist :-

<img width="250" height="124" alt="image" src="https://github.com/user-attachments/assets/f77b1880-c5a5-4796-b25b-16e22dc23c4c" />

Now we write spice netlist for above circuit :-

<img width="231" height="155" alt="image" src="https://github.com/user-attachments/assets/d8cf5e70-be93-4daf-acc2-ee82b4b60d40" />

M - mosfet R - resistor

Name - nodes - value

DGSS - drain gate source substrate (ordered)

if node = 0 just write 0 instead of name

nmos - comes from technology file

W = __ L = ___ dimensions

<img width="538" height="172" alt="image" src="https://github.com/user-attachments/assets/217e1c1e-6818-4fb7-bb3b-582b2a5a1c42" />

Technology File :-
 Model parameters.

 <img width="287" height="207" alt="image" src="https://github.com/user-attachments/assets/345ffb00-f247-4d40-bb83-62d071a388f3" />

<img width="296" height="52" alt="image" src="https://github.com/user-attachments/assets/d579064f-239a-4857-9eea-f95833d8a646" />

Everythng packaged like this :- <img width="266" height="145" alt="image" src="https://github.com/user-attachments/assets/3436b31a-c6d3-431d-b28f-0afd74714c70" />

Simulations Commands :- 























