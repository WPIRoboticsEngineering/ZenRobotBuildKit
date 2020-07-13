<img src="photos/whole-kit-layout.jpg" width="300">

# 0) Start with power disconnected

Do not put in batteries until the instructions say to. Do not skip around, do these in order. 

Do not plug in the USB until the instructions say to. 

# 1) Assemble the Chassis Electronics

We will be wiring this module:

https://www.pololu.com/product/3543

to our ESP32. 

First, place the (1x6) socket headers in the motor/encoder holes closest to the edges of the board.

<img src="photos/headerForEncoder.jpg" width="300">

Then solder the headers for the motors to the Driver Board. You will want to be sure that the sockets are reasonably vertical; otherwise, the motors might not fit correctly. The easiest way to do that is to solder one pin of each header and then check that it's vertical before soldering the other five pins.

<img src="photos/solderEncoderHeaders.jpg" width="300">

Put the dual-battery contacts into the chassis:

<img src="photos/contacts.jpg" width="300">

Flip the Romi over and set the single battery contacts in place. Squeeze the spring to fit the negative terminal into its hole:

<img src="photos/squeeze.jpg" width="300">

Add the positive terminals:

<img src="photos/bothContact.jpg" width="300">

Before you go to the next step, check that the terminals are aligned properly, For each battery compartement, the negative (spring) terminal should be opposite a positive (no-spring) terminal. Further, the terminals should protrude about 1/8" above the plastic (you should be able to just see the hole in the terminal above the plastic).

With your 4 battery contacts in place, place the driver board on top. Each terminal should protrude just a bit above the driver board.

<img src="photos/4Contacts.jpg" width="300">

Solder the battery contacts. They have a lot of thermal mass, so you may have to hold the soldering iron on them for a bit.

<img src="photos/solderBatt.jpg" width="300">

Add the motor Clips to both sides

<img src="photos/motorClip.jpg" width="300">

Slide the motor in, being careful to get the motor pins into the receiving socket you soldered earlier:

<img src="photos/motorAllignment.jpg" width="300">

Once aligned, fully seat the motor

<img src="photos/motorSeat.jpg" width="300">

Do the same for the other motor

<img src="photos/bothMotorsDone.jpg" width="300">




# 2) Add Long Wires to Driver Board

All wires should be 100 to 200 mm long. 

Be sure to use sane color codes. 
 * White for 5v
 * Red for 3.3v
 * Black for ground
 * Green for Motor PWM
 * Orange for Motor Direction
 * Yellow for encoder signals
 
The pins that need wires are as follows:

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
 
<img src="photos/solderWires.jpg" width="300">

# 3) Add Line Sensor and Breadboard

<img src="photos/1.jpg" width="300">
<img src="photos/2.jpg" width="300">
<img src="photos/3.jpg" width="300">
<img src="photos/4.jpg" width="300">
<img src="photos/5.jpg" width="300">
<img src="photos/6.jpg" width="300">

 
# 4) Wire up the ESP32
 
 * VPU   to 3v3
 * VCC MD to VUSB
 * GND to GND on the Esp32
 * ~SLP   to GND to disable, floating to enable, start with it disabled
 
 <img src="photos/7.jpg" width="300">
 <img src="photos/8.jpg" width="300">
 <img src="photos/9.jpg" width="300">
 <img src="photos/10.jpg" width="300">
 <img src="photos/11.jpg" width="300">
 

 
# 5) STOP and verify this is correct

Use your multi-meter to check that:

1) 5v and Gnd are NOT  connected
1) 5v and 3.3v are NOT connected 
1) 3.3v and GND are NOT connected
1) GND on the driver board and GND on the ESP32 ARE connected

# 6) Add the protection diodes 

The stripe side goes towards the encoder, the other side goes into ground. These clamp the 5v encoder lines to below 3.3v (nominally 2v high)

<img src="photos/12.jpg" width="300">

Check that you have the direction correct by putting the volt meter from encoder line to ground. Move the encoder wheel by hand to see the voltage go from 0v to 2v. If it clamps belo0.2v, then you have it in backwards.

Once verified, do the other 4 the same way

<img src="photos/13.jpg" width="300">



# 7) Add encoder GPIO lines
 * ELA to GPIO 27
 * ELB to GPIO 26/A0
 * ERA to GPIO 32
 * ERB to GPIO 14
 
 <img src="photos/15.jpg" width="300">
 
 
# 8) Add motor control GPIO lines
 * Left PWM to GPIO 13
 * Left DIR  to GPIO 4/ A5
 * Right PWM to GPIO 12 
 * Right DIR to GPIO 25/A1
 
 <img src="photos/16.jpg" width="300">
 <img src="photos/17.jpg" width="300">
 
# 9) add the riser plate

<img src="photos/19.jpg" width="300">

 
# 10) Power up and test Voltages

Plug in the Esp32 USB cable and add the batteries. 

1) Check 5v pin is at 5v +-0.1v
1) Check 3.3v pin is at 3.3v +-0.1v
1) Power on the battery and unplug the USB
1) Check 5v and 3.3v again
 
# 11) Program the Esp32 with the Motor Test Example


Plug the USB back in. Make sure the Motor ~SLP pin is in GND. 


Open Arduino IDE and program the example 

```
RBE1001Lib/MotorTest
```

Open the serial monitor after programming. 

After programming, take ~SLP and connect it to an open breadboard rail. One motor should start moving.

Change the example to check the other motor. 
 
