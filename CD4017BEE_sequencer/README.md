# CD4017BEE Sequencer IC
CD(Counter/Divider) 4017 BEE


![](https://github.com/L4COUR/Demystifying-DD-LAB-s-IC-s/blob/master/CD4017BEE_sequencer/CD4017BEE.jpg)

### Pin 1-7 & pin 9-11:
- Pin-1: It is the output 5. It goes high when the counter reads 5 counts.
- Pin-2: It is the output 1. It goes high when the counter reads 0 counts.
- Pin-3: It is the output 0. It goes high when the counter reads 0 counts.
- Pin-4: It is the output 2. It goes high when the counter reads 2 counts.
- Pin-5: It is the output 6. It goes high when the counter reads 6 counts.
- Pin-6: It is the output 7. It goes high when the counter reads 7 counts.
- Pin-7: It is the output 3. It goes high when the counter reads 3 counts.
</br>
- Pin-9: It is the output 8. It goes high when the counter reads 8 counts.
- Pin-10: It is the output 4. It goes high when the counter reads 4 counts.
- Pin-11: It is the output 9. It goes high when the counter reads 9 counts.
</br>
- Pin-8: GND (Ground)
- Pin-16: Vdd (+5 volts)
</br>
- pin-12: CO (Cascade Out) 
  - This pin is used to cascade the CD4017BEE with other 4017 IC's enabling a larger count-nr. 
  ex. The current 4017 IC counter can only reach a maximum of 10 steps when all the pins are used, however cascading with yet another 4017 ICs could double the amount of steps in the sequence.
</br>  
- pin-13: EN (Disable Pin)
  - This pin is normally set to GND or Low, if it recieves a HIGH, then the circuit will stop receiving counts effectively stopping the sequence
</br> 
- pin-14: CLK (Clock Input)
  - This is the pin which advances the counter when given an input
</br>  
- pin-15: MR (Master Reset)
  - This pin should normally be set to LOW in order for the counter to advance, given a HIGH voltage it will reset the counter back to 0.
</br> 


### sources:
- https://youtu.be/PVDnh9KYicA?t=831
- http://www.ti.com/lit/gpn/cd4017b
- https://www.elprocus.com/ic-4017-pin-configuration-application/

