# ZenRobotBuildKit

Zen robotics build kit is a robot build system. Here are the BOM and CAD models.

<img src="photos/allDone.jpg" width="300">

# Set Up Our Version of Arduino

Hold off on installing an IDE. We'll tell you about IDEs in class on Monday. You can start soldering and building.

## VSCode Option

[Install VSCode and PlatformIO](https://github.com/WPIRoboticsEngineering/ZenVSCodeInstaller)

## Eclipse Option

[Install arduino for your platform with the ESP32 toolchain set up](https://github.com/WPIRoboticsEngineering/RobotInterfaceBoard/blob/master/InstallEclipse.md)


# Build the Romi

1) [Wire the Chassis -- 1001 only!](Esp32RomiWiring.md)

1) [Wire the sensors -- 1001 only!](wireSensors.md)

1) [Build the lifting Arm -- 1001 only!](lifter.md)

# RBE1001Lib Documentation

[RBE1001Lib Doxygen page](https://wpiroboticsengineering.github.io/RBE1001Lib/annotated.html)

# Connect to Wifi

Program the RCCTL example and follow [these instructions to connec to to network](https://github.com/madhephaestus/Esp32WifiManager#connect-to-wifi-network)

# BOM Source

## Tools Kit (Online only, suggested)
  
  1 x wire stripper https://www.pololu.com/product/1923
  
  1 x Digital Multi Meter https://www.sparkfun.com/products/12966
  
  1 x soldering iron  https://www.sparkfun.com/products/14456
  
  1 x soldering stand  https://www.sparkfun.com/products/9477
  
  1 x spool of solder lead free https://www.digikey.com/product-detail/en/aven-tools/17551LF/243-1341-ND/5252791
  
  1 x spool of solder wick https://www.sparkfun.com/products/9327
  
  1 x spring scale https://www.elexp.com/71ea7-g63spring-scale-tubular-5000g-yel.html
  
  1 x x86_64 PC running Windows or Linux nativly
  * No MacOS (install windows dual-boot)
  * No Chromebooks (No way to get the software working)
  * No Microsoft Surfaces (if they are the ARM variant)
  

## Consumables Kit 

  Note that students only need a portion of the items here: e.g., they don't each need a wire spool kit -- they just need enough wire to wire their 'bot.

  1 x pack of zipties https://www.amazon.com/Cable-Nylon-Locking-Pieces-Black/dp/B07VRSQ6YL
  
  1 x roll double sided tape Foam tape https://www.amazon.com/Scotch-Mounting-0-75-inch-350-inches-110-LongDC/dp/B009NP1OBC
  
  1 x Wire Kit https://www.amazon.com/REXQualis-Breadboard-Assorted-Prototyping-Circuits/dp/B081H2JQRV
  
  1 x Wire spool kit https://www.amazon.com/StrivedayTM-Solid-Electric-gauge-26-2ft/dp/B077HRKYB1
  
  ```alternate   https://www.mouser.com/ProductDetail/Adafruit/1311?qs=GURawfaeGuBbUKgxUfZ%252BxQ%3D%3D```

## ESP32 Processor Kit CD-2021

1 x ESP32-DevKitC-VB https://www.digikey.com/product-detail/en/espressif-systems/ESP32-DEVKITC-32D/1965-1000-ND/9356990

1 x ZenDriver board (Provided by B Star contract manufacturer)

1 x USB cable https://www.amazon.com/NetDot-Magnetic-Charging-Transfer-Compatible/dp/B07QDS3CHN bought in packs of 3

1 x Breadboard https://www.pololu.com/product/4000 (specifically this one, as it has mounting holes)
     


## ESP32 Processor Kit AB-2020

  1 x ESP32-DevKitC-VB https://www.digikey.com/product-detail/en/espressif-systems/ESP32-DEVKITC-32D/1965-1000-ND/9356990
  
  1 x USB cable https://www.amazon.com/NetDot-Magnetic-Charging-Transfer-Compatible/dp/B07QDS3CHN bought in packs of 3

  1 x Breadboard https://www.pololu.com/product/4000 (specifically this one, as it has mounting holes)
  
  1 x #3543 Motor Driver and Power Distribution Board for Romi Chassis = 19.95
  
  7 x Zener Diode https://www.digikey.com/products/en?keywords=BZX55B3V9-TAPGICT-ND
  
  3 x 1x06 Male Header https://www.digikey.com/products/en?keywords=2057-PH1-06-UA-ND
  
  2 x 1x03 Female Header https://www.digikey.com/product-detail/en/sullins-connector-solutions/PPPC031LFBN-RC/S7036-ND/810175
  
  2 x 1x04 Male Header https://www.digikey.com/products/en?keywords=%202057-PH1-04-UA-ND
  
  4 x 1x19 Female Header https://www.digikey.com/products/en?keywords=PPTC191LFBN-RC
  
  1 x 1x02 male header https://www.digikey.com/product-detail/en/adam-tech/PH1-02-UA/2057-PH1-02-UA-ND/9830266
  
  1 x 1x04 Female Header https://www.digikey.com/product-detail/en/sullins-connector-solutions/PPPC041LFBN-RC/S7037-ND/810176
  
  1 x 1x03 Male Header https://www.digikey.com/product-detail/en/sullins-connector-solutions/PREC003SAAN-RC/S1012EC-03-ND/2774851
  
  1 x Romi Battery Contact Set https://www.pololu.com/product/3540

  1 x 1 kOhm resistor (reassigned from Sensors Kit -- only needed for shim board)
  
  1 x jumper

  1 x Custom PCB https://github.com/WPIRoboticsEngineering/1001-romi-processor-shim
  
```
  This will be produced and provided by the Robotics Department 
  ```
 
  
## 32u4 Processor Kit

  1 x Romi 32U4 Control Board https://www.pololu.com/product/3544
  
  3 x 1x6 socket: https://www.pololu.com/product/1016
  
  2 x 1x9 socket: https://www.pololu.com/product/1019 (2001 students: you'll also need the 3rd 1x9 socket in the Sensors Kit.)
  
  1 x 1x40 breakaway pins: https://www.pololu.com/product/1065
  
  1 x USB cable https://www.amazon.com/NetDot-Magnetic-Charging-Transfer-Compatible/dp/B07QDS3CHN bought in packs of 3

  1 x Breadboard https://www.pololu.com/product/4000 (specifically this one, as it has mounting holes)
  
  1 x Side-entry screw terminal: https://www.pololu.com/product/2491 (comes in packs of three -- each kit needs one)
  


## Chassis Kit

  1 x #3660 Romi Chassis Kit/Encoders (BULK special purchase)
  ```
  Low volume alternate source 
  
   1 x chassis kit https://www.pololu.com/product/3501
   1 x Romi Encoder Pair https://www.pololu.com/product/3542
  
  ```
  
  1 x #3560 Romi Chassis Expansion Plate - Black = 4.75
  
  1 x #3531 Romi Chassis Ball Caster Kit = 2.95 (color unimportant)
  
  1 x #1944 Aluminum Standoff: 1", 2-56 thread (4-pack): https://www.pololu.com/product/1944
  
  1 x #1943 Aluminum Standoff: 3/4", 2-56 thread (4-pack): https://www.pololu.com/product/1943

  1 x #2009 Aluminum Standoff: 1 1/2", 2-56 thread (4-pack): https://www.pololu.com/product/2009
  
  1 x 2-56 nut set https://www.pololu.com/product/1067
  
  1 x 2-56 x 1/4"long https://www.pololu.com/product/1955   

  1 x Servo with feedback https://www.pololu.com/product/3436
  
  1 x 2-56x 1.25" https://www.mcmaster.com/90272A087
  
  10 x 2-56x 3/4" https://www.mcmaster.com/90272A084
  
## Sensors Kit
  
  1 x line sensor array (6 x 8mm): https://www.pololu.com/product/4246
  
  1 x ultrasonic https://www.sparkfun.com/products/15569 
  
  1 x wire for ultrasonic https://www.sparkfun.com/products/10369

  2 x photoresistor: https://www.sparkfun.com/products/9088
  
  1 x yellow LED
  
  1 x 330 Ohm resistor

  2 x 2.2 kOhm resistor
  
  (1) 1x9 socket: https://www.pololu.com/product/1019 
  
  1 x potentiometer Digikey PN 3310R-125-103L-ND
  
  1 x IR receiver: https://www.pololu.com/product/2471 

  1 x IR remote: https://www.pololu.com/product/2777
  
## 2001 Add On kit

 1 x Motor With Encoder https://www.sparkfun.com/products/16413
 
 1 x Motor Driver - Dual TB6612FNG https://www.sparkfun.com/products/14450
 
 1 x transistor Digikey https://www.digikey.com/en/products/detail/on-semiconductor/2N2222/33077
 
 1 x relay Electronix Express PN: 22RCLR5V
  
 1 x Diode digikey 	1N4007-TPMSTR-ND
 
## 2002 Add On Kit
 
 1 x Cable for Sharp IR sensor: https://www.sparkfun.com/products/13685
 
 1 x SharpIR bracket https://www.pololu.com/product/2677
 
 1 x SharpIR proximity sensor https://www.pololu.com/product/136
  
 <!--(tentative) 1 x ToF distance sensor: https://www.pololu.com/product/2490-->
 
 
    
