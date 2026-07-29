# Wireless Telescope Control Using Recycled Starlink Gen2, ESP32C3 and BLE Xbox controller

![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/Telescope.png?raw=true)

## 🚀 Summary

 **26-7-26 This is WIP a developing project**
Being frustrated with aligning a cheap Telescope and keeping it on target a upgrade is required

 - The Starlink Gen 2 Antenna has a very strong gimble motor setup. These have anamzing amount of torq at low RPM 12v
 - Have remove the Antenna part and kept the base and motor assembly
 - Have designed some parts in Fusion 360 and 3d printed to make Telecope mount onto Starlink Assembly and Tripod
 - Useing L298 H Bridge to interface the 2 motors to ESP32C3
 - Useig BLE Gamecontroler (Xbox) to move and focus
 - Exploring connetion to Stellarium Astronomy Software API
 - Cheap USB camera lens camera
 - See what we get

## 📦 Build & Installation

![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/StarLink2.JPG?raw=true)
![](https://github.com/KiwiPlastic/Telescope/blob/main/Images/StarLink3.JPG?raw=true)

### Hardware: 
    1 x ESP32-C3
   
### Diagrm 
New Diagram to Come 

![circuit](https://github.com/KiwiPlastic/Wall-E_ESP32-C3_BLE_Gamepad_Ctrl/blob/main/Images/Wall-E%20CCT.png?raw=true)

## 🛠️ Usage
To be updated
### BLE Gamepad - Xbox controler - Button Map :-
    Tracks turn left/right  	Left Stick X (hoz)      
    Tracks forward/back       Left Stick Y (Vert) 
    Head rotation           	Right Stick X
    Head Up/Down            	Right Stick Y
    Neck Bottom             	Button A + Dpad Up/Dwn
    Lhs Eye                 	Button X + Dpad Up/Dwn
    Lhs Eyebrow             	Button X + Dpad Left/Right
    Rhs Eye                 	Button B + Dpad Up/Dwn
    Rhs Eyebrow             	Button B + Dpad Left/Right
    Bay Door Open/Close      	Button Y + Dpad Left Right
    Left Arm               	  Left Trigger  + Dpad Up/Dwn
    Right Arm              	  Right Trigger + Dpad Up/Dwn
    Play Sound              	Left Bumper + Dpad Left/Right - can crash
    Motor dead zone         	Left Bumper + Dpad Up/Dwn - 0 to 250
    LEDS move               	Right Bumper + Dpad Left/Right - loop x 4
    Steering Offset         	Right Bumper + Dpad Up/Dwn -  -100 to 100
    Animation Number          ViewButton +  Dpad Up/Dwn
    Automonus Mode    	      MenuButton On/Off toggel
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
