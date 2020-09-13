# Ultrasonic Range Finder

The shim board comes with a 4-pin port for connecting your ultrasonics sensor. Using your 4-wire cable connect the sensor to the port. Common practice is to use green for GND and red for power, which matches nicely with the cable.

Unfortunately, due to an oversight (from a change in ESP32 version), the pins that are wired to the ultrasonic don't have the necessary functionality, so you'll need to add wires to connect pin 16 to pin 22 and pin 17 to pin 32. You can just use the sockets in the shim board.

# Line Sensors

Vcc to 3.3v 

Gnd to Gnd

Sensor 3 to GPIO 36/A4

Sensor 9 to GPIO 39/A3

<img src="photos/18.jpg" width="300">


# Servo

Servo Black to Ground

Servo Red to 5v/VUSB

Servo White to GPIO 33

Servo Green to GPIO 34/A2
