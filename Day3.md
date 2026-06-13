D3SK1
-----

Spice desk
--------------
- component connectivity
- identify and name nodes
- component values

<img width="262" height="229" alt="image" src="https://github.com/user-attachments/assets/21d86050-c5c8-4015-b714-5a50b6a3b6c4" />

(M1 is PMOS , M2 is CMOS)

Source of Pmos ro vdd and of nmos to vss.

Remember : DGSS - drain gate source substrate

*** MODEL Description ***

*** Netlist Description ***

M1 out in vdd vdd pmos L = 0.375u W = 0.25u

M2 out in  0 0 nmos L = 0.375u W = 0.25u

cload out 0 10f (f - femtofarad)

Vdd vdd 0 2.5 

Vin in 0 2.5

*** Simulation Commands ***

.op - Calculates a single, static set of DC conditions (voltages at every node and currents through every branch) for a circuit. It treats capacitors as open circuits and inductors as short circuits.
.dc -  Performs operating point analyses repeatedly while sweeping an independent voltage or current source across a specific range.

.dc Vin 0 0 2.5 0.05

*** .imclude libname ***

.LIB ----------------
.end

<img width="413" height="314" alt="image" src="https://github.com/user-attachments/assets/e8562adb-dbe4-4a55-ba50-7d8c9de60b32" />

Changing length of pmos -

<img width="403" height="314" alt="image" src="https://github.com/user-attachments/assets/4c5a8f8f-1ae5-47bd-bad5-60e1bb54fe54" />

Lab :-

<img width="208" height="238" alt="image" src="https://github.com/user-attachments/assets/188800da-087e-4110-869a-b98b19541b0a" />

 F or CmOS Inverter
<img width="951" height="381" alt="image" src="https://github.com/user-attachments/assets/5fc20d5c-7268-47d9-87f9-218605ffa601" />


CMOS Inverter netlist

<img width="274" height="292" alt="image" src="https://github.com/user-attachments/assets/ec93d82d-4991-4d9d-b090-4103187b2b9e" />

 .parameter temp =27 - Sets simulation temperature to 27°C (room temperature)

 .lib "sky130_fd_pr/models/sky130.lib.spice" tt

 sky130_fd_pr - SkyWater 130nm Foundry Primitive library
 sky130.lib.spice - SPICE model file for transistors
 tt - Typical - Typical process corner (nominal PMOS + NMOS) 
 other eg - ff , ss ,fs,sf (fast/slow)
 <img width="509" height="197" alt="image" src="https://github.com/user-attachments/assets/45683ec6-bcb8-45d2-8c62-eb9be60be661" />

Vin in 0 PULSE(0V 1.8V 0 0.1ns 0.1ns 2ns 4ns)

<img width="359" height="214" alt="image" src="https://github.com/user-attachments/assets/fb3998a0-4bf0-44d8-b4cd-e3c4442d5436" />

.tran 1n 10n - Transient analysis — simulates for 10 nanoseconds with 1ns time steps
You'll see ~2.5 complete clock cycles

.control
run
.endc
Runs the simulation automatically when NGSpice starts


<img width="421" height="302" alt="image" src="https://github.com/user-attachments/assets/ea670e76-416c-4e62-9a8a-bbac9b1ab906" />

Dynamic characteristics(rise and fall delay) of cmos inverter circuit for wp/lp = wn/ln

<img width="560" height="324" alt="image" src="https://github.com/user-attachments/assets/7dd2b96e-e752-4f4d-b1ac-55df250a3be6" />

measure propagation delay (tpLH) — the time between:

Input crossing VDD/2 = 0.9V (falling)
Output crossing VDD/2 = 0.9V (rising

<img width="318" height="137" alt="image" src="https://github.com/user-attachments/assets/6c34a2a5-b81d-41fe-96bf-59b542097542" />

plot out vs time in

<img width="697" height="383" alt="image" src="https://github.com/user-attachments/assets/d4374b9e-7118-4925-bcdd-acf67e127eae" />

<img width="445" height="377" alt="image" src="https://github.com/user-attachments/assets/d898b4ab-35c5-4ffb-a28e-938dccf0c044" />


<img width="648" height="371" alt="image" src="https://github.com/user-attachments/assets/5d5e2a1c-1d52-4192-aa0c-c53967763f1f" />

latest reading for in







