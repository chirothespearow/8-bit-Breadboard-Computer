# 8-bit-Breadboard-Computer
An 8-bit breadboard computer inspired by Ben Eater

# Clock Module
![cclock](https://user-images.githubusercontent.com/44639543/183112306-f6bdc335-b237-4ec1-9105-b7728daf1436.jpg)
## Components Used:  
3 x LM-555 Timer ICs  
1	x 74LS04 Hex inverter  
1	x 74LS08 Quad 2-input AND gate  
1	x 74LS32 Quad 2-input OR gate  
1	x Momentary tact switch  
1	x SPST slide switch  
1	x 1MΩ potentiometer  
2 x	0.01µF capacitors  
1	x 0.1µF capacitors  
1	x 1µF capacitors  
Resistors
LEDs
## Modes
Monostable and Astable modes are available, and can be switched accordingly.

# Registers and ALU
![alu](https://user-images.githubusercontent.com/44639543/183114704-f7318399-a0bd-4497-88e9-c204d0eb8e43.jpg)
## Components Used:  
2	x 74HC86 Quad XOR gate  
6	x 74LS173 4-bit D register  
4	x 74LS245 8-bit bus transceiver  
2	x 74LS283 4-bit binary adder  
Resistors  
LEDs

## Logic
The Red LEDs represent the values present in the two registers, while the Yellow LEDs represents the output of the ALU. XOR chips are used to subtract the numbers by virtue of two's complement. The registers have a load signal which is active low, and controls whether data can be loaded into the register or not. The D-registers only load data at the rising edge of the clock pulse (obtained from the clock module). The 74LS245 is a tri-state bus transceiver that allows the registers to read data from the bus, and has an enable signal (active low) to control it. The 74LS283 is used to add the two register values.

In the image provided above, the numbers 143 (10001111) and 127 (01111111) are added to give 14 (00001110), which can be confirmed with a binary calculator. 
(overflow occurs)

# RAM and program counter
Coming soon

# Control Logic
Coming soon
