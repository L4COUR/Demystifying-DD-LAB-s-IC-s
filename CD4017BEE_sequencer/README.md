# CD4017BEE Sequencer IC
CD(Counter/Divider) 4017 BEE


![](https://github.com/L4COUR/Demystifying-DD-LAB-s-IC-s/blob/master/CD4017BEE_sequencer/CD4017BEE.jpg)

#### Pin 1-7 & pin 9-11:
- Pin-1: It is the output 5. It goes high when the counter reads 5 counts.
- Pin-2: It is the output 1. It goes high when the counter reads 0 counts.
- Pin-3: It is the output 0. It goes high when the counter reads 0 counts.
- Pin-4: It is the output 2. It goes high when the counter reads 2 counts.
- Pin-5: It is the output 6. It goes high when the counter reads 6 counts.
- Pin-6: It is the output 7. It goes high when the counter reads 7 counts.
- Pin-7: It is the output 3. It goes high when the counter reads 3 counts.
</br></br>
- Pin-9: It is the output 8. It goes high when the counter reads 8 counts.
- Pin-10: It is the output 4. It goes high when the counter reads 4 counts.
- Pin-11: It is the output 9. It goes high when the counter reads 9 counts.
</br></br>
#### Pin 8 & 16:
- Pin-8: GND (Ground)
- Pin-16: Vdd (+5 volts)
</br></br>
#### Pin 12-15:
- pin-12: CO (Carry Out) 
  - This pin is used to cascade the CD4017BEE with other 4017 IC's enabling a larger count-nr. 
  ex. The current 4017 IC counter can only reach a maximum of 10 steps when all the pins are used, however cascading with yet another 4017 ICs could double the amount of steps in the sequence.
</br>  </br>
- pin-13: EN (Disable Pin)
  - This pin is normally set to GND or Low, if it recieves a HIGH, then the circuit will stop receiving counts effectively stopping the sequence
</br> </br>
- pin-14: CLK (Clock Input)
  - This is the pin which advances the counter when given an input
</br>  </br>
- pin-15: MR (Master Reset)
  - This pin should normally be set to LOW in order for the counter to advance, given a HIGH voltage it will reset the counter back to 0.
</br> </br>

## Getting started with CD4017BEE

### 1: testing if the chip is defekt

- connect pin-16 to a positive voltage source, next, connect pin-8 to ground
- use an LED (coupled with a resistor) to check if the chip works by connecting the LED to pin-3. if the LED lights up you are good to go, if it doesn't then you are probably using a defekt chip.

[Insert picture of testing the chip]

### 2: deciding what to build with the chip

There is a lot of different projekt that could be build using this chip. for simplicity's sake I have chosen to build a very simple circuit that besides the chip consist of; 8 LED (+resistors), 1 button, and some wires.

The idea is to build a ciruit, that at each button press advances the 8 step sequence, we will be using the same schematic from [1]. By building this you should get a pretty good idea of what this chip is all about.

### 3: setting up the circuit

![Insert fritzing Schematic](https://github.com/L4COUR/Demystifying-DD-LAB-s-IC-s/blob/master/CD4017BEE_sequencer/CD4017BEE_circuit_tutorial.png)

connect all the components acording to the schematic above, and make sure that everything is connected correctly. 

### 4: See if it is working

![](https://github.com/L4COUR/Demystifying-DD-LAB-s-IC-s/blob/master/CD4017BEE_sequencer/4017-circuit.gif)


### sources:

- [1] https://youtu.be/PVDnh9KYicA?t=831
- http://www.ti.com/lit/gpn/cd4017b
- https://www.elprocus.com/ic-4017-pin-configuration-application/

