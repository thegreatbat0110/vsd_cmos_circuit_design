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














