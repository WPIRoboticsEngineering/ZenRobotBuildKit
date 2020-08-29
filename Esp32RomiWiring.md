# Step 0 Learn to Solder (Click on image to play on YouTube)

[![Alt text](https://img.youtube.com/vi/FWBCbFPXJLg/0.jpg)](https://www.youtube.com/watch?v=FWBCbFPXJLg)

# Step 1 Lay out your electronics

<img src="photos/shim/0001.jpg" width="300">

# Step 2 Solder in the 10k Resistor

All components -- resistors, diodes, and sockets -- go on the top (silk screen) side of the shim board. 

<img src="photos/shim/0003.jpg" width="300">

Solder them from the bottom.

<img src="photos/shim/0004.jpg" width="300">

# Step 3 Solder in the Diodes

BE CAERFUL to line up the black stripe with the stripe in the silk screen. 

They are made of a bead of glass, be very careful with them.

<img src="photos/shim/0005.jpg" width="300">
<img src="photos/shim/0006.jpg" width="300">

# Step 4 Solder the ESP32 Sockets

Start by placing the sockets on your processor

<img src="photos/shim/0007.jpg" width="300">
<img src="photos/shim/0008.jpg" width="300">
<img src="photos/shim/0009.jpg" width="300">

then insert the sockets into the Shim.

<img src="photos/shim/0011.jpg" width="300">

Flip it over and solder the pins

<img src="photos/shim/0012.jpg" width="300">

# Step 5 Solder the rest of the headers as shown

<img src="photos/shim/0025.jpg" width="300">

# Step 6 Solder the headers that come with the Driver Board

When soldering in the 1x6 sockets, be sure to use the short ones that came in the bag with the Driver Board. Be sure that the sockets are fully seated on the board and perpendicular to it; otherwise, you will have trouble connecting the motors later. Best to solder one connection and then check before you solder the other five.

<img src="photos/shim/0026.jpg" width="300">
<img src="photos/shim/0027.jpg" width="300">

The sockets go in the outer positions.

<img src="photos/shim/0030a.jpg" width="300">

<img src="photos/shim/0028.jpg" width="300">

# Step 7 Dry fit the headers between the Driver and the Shim

Start with both boards.

<img src="photos/shim/0030.jpg" width="300">

Add four sets of pins, as shown. The short leg of the pins go into the board; the long legs stick up.

<img src="photos/shim/0034a.jpg" width="300">


# Step 8 Place the Shim on and tape it in place before soldering

<img src="photos/shim/0031.jpg" width="300">
<img src="photos/shim/0032.jpg" width="300">

# Step 9 Solder the Driver Board ONLY (Not the red shim yet)

<img src="photos/shim/0033.jpg" width="300">

Remove the shim after soldering to check the joints

<img src="photos/shim/0034.jpg" width="300">

# Step 10 Add the battery tabs to the Chassis

<img src="photos/shim/0036.jpg" width="300">
<img src="photos/shim/0037.jpg" width="300">
<img src="photos/shim/0038.jpg" width="300">

# Step 11 Solder the Battery Tabs

The tabs should protrude roughly 1/16 inch above the Driver Board.

<img src="photos/4Contacts.jpg" width="300">

# Step 12 Add line sensor

(Skip this step for now.)

# Step 13 Solder the Shim to the Driver Board

Slip the shim board back on the pins you solder to the Driver Board in Step 9. Be sure the shim is fully seated before soldering (use tape again). The long pins will protrude well above the shim. That's OK.

# If you are in any doubt about your soldering work so far, have someone look over your soldering work (SA, LA, TA, faculty, lab manager, friends, romans, countrymen...).

Once you solder the shim board to the Driver Board, repairing bad solder joints will range from troublesome to impossible.

<img src="photos/shim/0039.jpg" width="300">
<img src="photos/shim/0040.jpg" width="300">

# Step 14 Add Motor Mount Clips

Add the motor Clips to both sides

<img src="photos/motorClip.jpg" width="300">

Slide the motor in, being careful to get the motor pins into the receiving socket you soldered earlier:

<img src="photos/motorAllignment.jpg" width="300">

Once aligned, fully seat the motor

<img src="photos/motorSeat.jpg" width="300">

Do the same for the other motor

<img src="photos/bothMotorsDone.jpg" width="300">


# Step 15 Power up and test Voltages

Put your ESP32 into the sockets in the shim board. Pay close attention to orientation -- the shim has text for which end the USB connector is on. Plug in the USB cable. 

1) Check that the 5V pin is at 5+-0.1 V
2) Check 3.3V pin is at 3.3+-0.1 V
3) Add batteries, power on the Driver Board and unplug the USB
1) Check 5V and 3.3V pins again
 
# Step 16 Program the ESP32 with the Encoder Test Example


Plug the USB back in.  


Open your IDE of choice and program the example 

```
RBE1001Lib/EncoderTest
```

Open the serial monitor after programming. Gently roll the Romi forward and backward (the shim board faces the front) and verify that the wheels count up when rolling forward and down when backwards.

# Step 17 Program the ESP32 with the Motor Test Example

Place the jumper on the two pins marked ???. This will connect the "sleep" pin to ground so your motors can't spin.

Open and upload the example

```
RBE1001Lib/MotorTest
```

After programming, *pick up your robot* and pull the sleep jumper out of the shim. The motors will start spinning. It may jump if there is a wiring issue, so do not do this with the robot on the table or it may drive off. Pick it up!


# Step 18 add the riser plate

Use 2x of your 1 inch standoffs to attach the riser using the recessed screws as shown. Look for the screw head near each motor. Attach the standoff below with a nut from inside the battery compartment. 

Use the 1 1/2 inch standoffs in the back to secure the back of the riser plate. 

<img src="photos/19.jpg" width="300">

# Step 19 Add the casters

<img src="photos/25jpg" width="300">
<img src="photos/26.jpg" width="300">
<img src="photos/27.jpg" width="300">
<img src="photos/28.jpg" width="300">
<img src="photos/29.jpg" width="300">

 
