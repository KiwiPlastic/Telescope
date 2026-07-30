# Telescope Goto Control, Using Recycled Starlink Gen2, ESP32C3 and Wireless BLE controller

![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/Telescope.png?raw=true)

## 🚀 Summary

 **26-7-26 This is WIP a developing project**
 
Being frustrated with aligning a cheap Telescope and keeping it on target a upgrade is required

 - The Starlink Gen 2 Antenna has a very strong gimble motor setup. These have anamzing amount of torq at low RPM 12v
 - Have remove the Antenna part and kept the base and motor assembly
 - Have designed some parts in Fusion 360 and 3d printed to make Telecope mount onto Starlink Assembly and Tripod
 - Useing L298 H Bridge to interface the 2 motors to ESP32C3
 - Useig BLE Gamecontroler (Xbox) to move and focus
 - Cheap USB Eyepeace camera MD-205 (this is the only part im actualy byeing, rest is stock and time)
 - Exploring connetion to Stellarium Astronomy Software API to use Goto function
 - SharpCap Image capture software may also suport Goto
 - ChatGPT conferims can orientate from Date/Time, GPS, IMU data, for orienation and then Goto
 - ChatGPT can provid calculations and interfacing suport
 - See what we get

## 📦 Build & Installation

**Research**

 - Cheap Telescope usage is not the best start, but this is a very low budget project.
 - This camera and Telescope are only suitable for planetery observations
 - The concepts of this design will allow multi choices of hardware 
 - Cheap Telscope Improvements
   - Hang wight from center of tripod
   - Ensure all tripod bolts are tight
   - Ensure focuse tube is tight (no wobbel)
   - Service Focus Rack and pinnion adjustment - should slid firm but easy
 - Leave Telescope outside for 1/2 hour for temp to stabalize. Tube open
 - Takes half hour for night vision to be good. Sit in dark room while waiting
 - when you go outside, be fully prepeard with tools, food, water, warmth, chair

**USB Camera**
 - Found a ceap Eyepeace Camera MD-205 $25USD ( Aliexpress)
 - ![This vid is great, explaing these cameras](https://www.youtube.com/watch?v=IZJV7a9rAaU)
 - Useing Sharpcap v4, astro camera software. Was plug and play.

**Starlink Gen2 Atenna Base**

![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/StarLink2.JPG?raw=true)
![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/StarLink3.JPG?raw=true)

The stripped down Starlink Antenna

### Hardware: 
    1 x ESP32-C3
    1 x L298 Stepper motor / H Bridge
    1 x 3v to 5v level converter
    1 x 5 amp Buck
    1 x DFRobot IMU LHS303
    1 X GPS NEO6
    
### Diagrm 

![circuit](https://github.com/KiwiPlastic/Telescope/blob/main/Images/Telescope_CCT.png?raw=true)

## 🛠️ BLE Gamepad - Xbox Controler - Button Map

    Left Stick X (hoz)      
    Left Stick Y (Vert)  
    Right Stick X
   	Right Stick Y
    Button A + Dpad Up/Dwn
   	Button X + Dpad Up/Dwn
    Button X + Dpad Left/Right
    Button B + Dpad Up/Dwn
    Button B + Dpad Left/Right
    Button Y + Dpad Left Right
    Left Trigger  + Dpad Up/Dwn
    Right Trigger + Dpad Up/Dwn
    Left Bumper + Dpad Left/Right 
    Left Bumper + Dpad Up/Dwn 
    Right Bumper + Dpad Left/Right 
    Right Bumper + Dpad Up/Dwn 
    ViewButton +  Dpad Up/Dwn
    MenuButton On/Off toggel
    Dpad Up                 	adjust up
    Dpad Down               	adjust down
    Dpad Left               	adjust left
    Dpad Right              	adjust right
    Left Stick Button
    Right Stick Button
    ShareButton
    XboxButton

## 📜 License
Distributed under the MIT License. See `LICENSE` for more information.
