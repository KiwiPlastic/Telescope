# Telescope - ESP32C3 and Wireless BLE controller - Using Recycled Starlink Gen2 Antenna Motors & assembly
![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/Telescope.png?raw=true)

## 🚀 Summary
 
Being frustrated with aligning a cheap Telescope and keeping it on Target, a upgrade is required.

**Goals:**
  - To control Telescope via Xbox controler, to ensure stable Targetting
  - Get nice digital pictures of the Moon
  - Absolute minimal cost, as might not get into it

Angeleys MD-205 Eyepeace camera was the only thing purchased. This is the equivilent of the SV-205

All other parts ex stock

Alt-Azimuth Mount: It goes up and down (altitude) and left and right (azimuth)

Equatorial Mount: It has two axes, but one is tilted to match the angle of the Earth's axis

 **Starlink Gen 2 Antenna**
 - The Starlink Gen 2 Antenna has a very strong gimble motor setup. These have anamzing amount of torq at low RPM 12v
 - Have removed the Antenna part and kept the base and motor assembly. Use a grinder to open it up
 - Have designed some parts in Fusion 360 and 3d printed to make Telecope mount onto Starlink Assembly and Tripod
 
 **Electronics**  
 - ESP32C3 BLE WiFi 
 - L298 H Bridge to interface the 2 Starlink motors to ESP32C3
 - IMU (Future development)
 - GPS (Future development)
 - BLE Xbox Game controler as wireless handcontroler to initiate movement
 - Cheap USB Eyepeace camera Angeleyes MD-205 (this is the only part im actualy byeing, rest is stock and time)
 - SharpCap Image capture software
 - See what we get

 **Futre Developments**
 - IMU dadt output
 - GPS Data output
 - Orientate Telescope
 - ChatGPT conferims can orientate from Date/Time, GPS, IMU data, for orienation and then Goto
 - ChatGPT can provid calculations and interfacing suport
 - Tracking to compensate earths movement
 - Exploring connetion to Stellarium Astronomy Software API to use Goto function

## 📦 Build & Installation

**Research**
 - Cheap Telescope usage is not the best start, but this is a very low budget project.
 - The Eyepeace camera model and Telescope are only suitable for planetery observations, not deep space
 - Cheap Telscope Improvements
   - Hang wight from center of tripod
   - Ensure all tripod bolts are tight
   - Ensure focuse tube is tight (no wobbel)
   - Service Focus Rack and pinnion adjustment - should slid firm but easy
 - Leave Telescope outside for 1/2 hour for temp to stabalize. Tube open
 - Takes half hour for night vision to be good. Sit in dark room while waiting
 - when you go outside, be fully prepeard with tools, food, water, warm clothing, chair

**USB Camera**
 - Angeleys MD-205 200W Eyepeace camera $25USD ( Aliexpress)
 - CCD/CMOS 1080P
 - 8MP
 - 24bit RGB
 - Sensor Size: 1/2.7 inch
    
![This vid is great, explaning these cameras](https://www.youtube.com/watch?v=IZJV7a9rAaU)

 - Useing Sharpcap v4, astro camera software. Was plug and play

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
