# Ultrasonic Range Finder

The shim board comes with a 4-pin port for connecting your ultrasonic sensor. Using your 4-wire cable connect the sensor to the port. Common practice is to use green for GND and red for power, which matches nicely with the cable.

Unfortunately, due to an oversight (from a change in ESP32 version), the pins that are wired to the ultrasonic don't have the necessary functionality, so you'll need to add wires to connect pin 16 to pin 22 and pin 17 to pin 32. You can just use the sockets in the shim board.

# Line Sensors

Your shim board has two 3-pin connectors for line sensors. The arrangement is set up to work with individual line sensors, but it will also work with the line sensor array.

Connect the '+' terminal from one of the line sensor sockets to Vcc on the sensor array. Connect '-' to GND. You do note need to connect the '+' and '-' from the other sensor.

Connect the middle pin of each socket to your choice of sensors: 1, 3, 5, 7, 9, or 11. These correspond to each of the physical sensors on the working side of the sensor array. In the end, you'll want to choose two sensors that are roughly the width of the piece of tape you use for line following, but you can easily try different sensor elements. The sockets are connected to pins 36 (A4) and 39 (A3) on your ESP32.


# Servo

The shim board has a 4-pin connector for the servo. Connect the black wire (ground) on the servo cable to the '-' terminal. The red wire will connect to 5V and the white to the signal line (pin 33). Connect the green feedback wire to the last pin, pin 34 (A2).
