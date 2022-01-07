# Arduino Basic Projects
Arduino traffic light projects are a fun little project that you can build in less than an hour. Here's how to build your own using Arduino, and how to change the circuit to get the most out of it. <br>

**In addition to the basic Arduino, you will need:** <br>
3 x 220-ohm resistors <br>
Bread board <br>
Connecting cables <br>
Red, yellow and green LEDs <br>

**Basic Traffic Light Controller:** <br>
The changeLights function performs all the hard work. This rotates the traffic light through yellow and red, then back to green. As this gets called inside the loop function, the Arduino will run this code forever, with a 15-second pause every time. <br>

<h4>The changeLights function consists of four distinct steps:</h4> <br>

Green on, yellow off <br>
Yellow off, red on <br>
Yellow on, red on <br>
Green on, red off, yellow off<br>

These four steps replicate the process used in real traffic lights. For each step, the code is very similar. The appropriate LED gets turned on or off using digitalWrite. This is an Arduino function used to set output pins to HIGH (for on), or LOW (for off).<br>

After enabling or disabling the required LEDs, the delay makes the Arduino wait for a given amount of time. Three seconds in this case.
