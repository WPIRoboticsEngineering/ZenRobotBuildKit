# Ultrasonic Range Finder


Vcc to 5vv/VUSB

Gnd to Gnd

Echo to One side of a 2.2k resistor

The other side of the 2.2k Resistor to GPIO 22

Trig to GPIO 23

<img src="photos/21.jpg" width="300">
<img src="photos/24.jpg" width="300">


# Line Sensors

Your shim board has two 3-pin connectors for line sensors. The arrangement is set up to work with individual line sensors, but it will also work with the line sensor array.

Connect the '+' terminal from one of the line sensor sockets to Vcc on the sensor array. Connect '-' to GND. You do not need to connect the '+' and '-' from the other set of pins.

Connect the middle pin of each set to your choice of sensors: labelled 1, 3, 5, 7, 9, or 11 on the sensor array. These correspond to each of the physical sensors on the working side of the sensor array. In the end, you'll want to choose two sensors that are roughly the width of the piece of tape you use for line following, but you can easily try different sensor elements. The sockets are connected to pins 36 (A4) and 39 (A3) on your ESP32.


# Servo

The shim board has a 4-pin connector for the servo. Connect the black wire (ground) on the servo cable to the '-' terminal. The red wire will connect to 5V and the white to the signal line (pin 33). Connect the green feedback wire to the last pin, pin 34 (A2).
