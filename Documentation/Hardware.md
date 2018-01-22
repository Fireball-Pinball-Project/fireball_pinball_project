# Hardware
## Pinball Hardware
Pinball hardware is primarily driven by relatively strong magnetic coils, usually in the form of solenoids. They tend to run from 24V DC to 110V AC. 
The Fireball system uses two power supplies(PS) to supply 3 main voltages.
1. 24V Solenoid power - This PS supplies a single 24V source for powering the solenoids. This is a switching power supply, which means that the sudden current spike from a solenoid firing may look like a short and cause the PS to reset. This is remedied by buffering the output of the PS with a power filter board. The power filter board is described here: http://pinballmakers.com/wiki/index.php/OPP#Power_Filter_Board
2. ATX PS - This PS is a standard PC unit which supplies 12V and 5V for switches, LEDs and powering the Arduino controller.

### General Hardware descriptions
See this page for more information on the basics of pinball hardware: http://markgibson.zenfolio.com/fun-with-pinball/learn

## Controller Hardware
The controller system uses an Arduino Mega as the main controller. A controller manages the physical state of the board. It is responsible for reading switches and activating physical systems(solenoids, motors, lights, etc). 

## Arduino Microcontroller

## Open Pinball Project (OPP)
The Open Pinball Project(OPP) is an attempt to design a small, inexpensive controller system for pinball controllers. It utilizes a Cypress microntroller for the main board. http://pinballmakers.com/wiki/index.php/OPP
The Fireball project uses two boards from the OPP project. One is the Power Filter Board mentioned above. The other is a solenoid board: http://pinballmakers.com/wiki/index.php/OPP#Solenoid_Wing
The solenoid boards use high voltage MOSFETs to turn 24V sources on and off. See this for a description of how MOSFETs work: https://oscarliang.com/how-to-use-mosfet-beginner-tutorial/

