# Arduino
Arduino traffic light projects are a fun little project that you can build in less than an hour. Here's how to build your own using Arduino, and how to change the circuit to get the most out of it.

In addition to the basic Arduino, you will need:
3 x 220-ohm resistors
Bread board
Connecting cables
Red, yellow and green LEDs

Basic Traffic Light Controller:
The changeLights function performs all the hard work. This rotates the traffic light through yellow and red, then back to green. As this gets called inside the loop function, the Arduino will run this code forever, with a 15-second pause every time.

The changeLights function consists of four distinct steps:

Green on, yellow off
Yellow off, red on
Yellow on, red on
Green on, red off, yellow off
These four steps replicate the process used in real traffic lights. For each step, the code is very similar. The appropriate LED gets turned on or off using digitalWrite. This is an Arduino function used to set output pins to HIGH (for on), or LOW (for off).

After enabling or disabling the required LEDs, the delay makes the Arduino wait for a given amount of time. Three seconds in this case.
