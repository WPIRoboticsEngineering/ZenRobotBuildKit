# Assemble the Chassis Electronics

We will be wireing this module:

https://www.pololu.com/product/3543

to our ESP32. 

# Cut the Encoder Pull Up Trace

# Add Long Wires to Driver Board

All wires should be 100 to 200 mm long. 

Be sure to use sane color codes. 
 * White for 5v
 * Red for 3.3v
 * Black for ground
 * Green for Motor PWM
 * Orange for Motor Direction
 * Yellow for encoder signals
 
The pins that need wires are as follows:

 * VPU    ( the pull up high side that needs to go to 3.3v)
 * VCC MD (Our 5v regulated output from the batteries)
 * ~SLP   (to disable the motors)
 * Left PWM (PWM setting the speed of the left motor)
 * Left DIR  (Direction flag for the left motor)
 * Right PWM (PWM setting the speed of the right motor)
 * Right DIR (Direction flag for the right motor)
 * GND (Ground reference)
 * ELA ( Left encoder A)
 * ELB ( Left encoder B)
 * ERA ( right encoder A)
 * ERB ( right encoder B)
 
 # Wire up the ESP32
 
 * VPU   to 3v3
 * VCC MD to VUSB
 * ~SLP   to GND to disable, floating to enable
 * Left PWM to GPIO 5/SCK
 * Left DIR  to GPIO 4/ A5
 * Right PWM to GPIO 15 
 * Right DIR to GPIO 
 * GND (Ground reference)
 * ELA ( Left encoder A)
 * ELB ( Left encoder B)
 * ERA ( right encoder A)
 * ERB ( right encoder B)
 
