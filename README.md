# fossee-marathon
# Abstact
A Buck Converter is a DC-DC step-down converter that efficiently reduces a higher input voltage to a lower output voltage without dissipating excess energy as heat, unlike voltage regulators or Zener diodes. It achieves this by increasing the output current while maintaining nearly the same power level through high-speed switching and energy transfer using inductive and capacitive elements. The converter regulates the output voltage by controlling the duration of energy storage and release, ensuring stable and efficient operation. Due to its high efficiency and reliability, it is widely used in power supply circuits, battery-powered devices, and embedded electronic systems.
# Reference Circuit Details
The circuit diagram of the Buck Converter consists of a battery connected to a switch, inductor, diode, capacitor, and load resistor as shown in Fig 1. The switch, which may be a transistor or MOSFET, operates at a high switching frequency to control the energy flow from the input to the output. When the switch is ON, current flows from the battery through the inductor and the load, storing energy in the magnetic field of the inductor. When the switch is OFF, the inductor releases its stored energy through the diode, maintaining a continuous current through the load. The capacitor filters out voltage ripples, ensuring a smooth DC output. 
# Reference Circuit Diagram 
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Reference%20image.jpeg?raw=true)
# Reference Waveform 
![image alt](https://github.com/rithivkrishna/fossee-marathon/blob/main/Reference%20image.jpeg?raw=true)
