# fossee-marathon
# Abstact
A Buck Converter is a DC-DC step-down converter that efficiently reduces a higher input voltage to a lower output voltage without dissipating excess energy as heat, unlike voltage regulators or Zener diodes. It achieves this by increasing the output current while maintaining nearly the same power level through high-speed switching and energy transfer using inductive and capacitive elements. The converter regulates the output voltage by controlling the duration of energy storage and release, ensuring stable and efficient operation. Due to its high efficiency and reliability, it is widely used in power supply circuits, battery-powered devices, and embedded electronic systems.
# Reference Circuit Details
The circuit diagram of the Buck Converter consists of a battery connected to a switch, inductor, diode, capacitor, and load resistor as shown in Fig 1. The switch, which may be a transistor or MOSFET, operates at a high switching frequency to control the energy flow from the input to the output. When the switch is ON, current flows from the battery through the inductor and the load, storing energy in the magnetic field of the inductor. When the switch is OFF, the inductor releases its stored energy through the diode, maintaining a continuous current through the load. The capacitor filters out voltage ripples, ensuring a smooth DC output. 
# Reference Circuit Diagram 
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Reference%20image.jpeg?raw=true)
# Reference Waveform 
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/reference%20waveform.png?raw=true)
# Simulation using Esim
## Schematic
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Schematic.png?raw=true)
## Source Details
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Source%20Details.png?raw=true)
## Transient Settings
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Analysis.png?raw=true)
## Device Modelling
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Device%20Modelling.png?raw=true)
## Netlist 
*
.title KiCad schematic
M1 in vsw Net-_D1-Pad2_ Net-_D1-Pad2_ eSim_MOS_N
v2 vsw GND pulse
U1 in plot_v1
v1 in GND DC
U2 vsw plot_v1
C1 Net-_C1-Pad1_ GND 10u
R1 GND out 500
U4 Net-_C1-Pad1_ out plot_i2
L1 Net-_L1-Pad1_ Net-_C1-Pad1_ 1.5m
D1 GND Net-_D1-Pad2_ eSim_Diode
U3 Net-_D1-Pad2_ Net-_L1-Pad1_ plot_i2
U5 out plot_v1
.end

