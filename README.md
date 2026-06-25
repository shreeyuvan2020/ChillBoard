 # The Chillboard
 ## The perfect ergonomic keyboard for chilling
 ## Features
 - Uses Xiao NRF52840 for low power usage and BLE capabilities
 - Wireless design with a 2000 mAh battery and BLE
 - CPG1350 hotswap sockets for customizabilty
 - Low profile choc switches for portability
 - Neopixel backlighting for layer switching
 - OLED panel for battery percentage
 - Tray mounted for easy assembly
 - Rotary encoder for volume control
 - PIR sensor for energy conservation
 - Ortholinear layout with a thumb cluster to reduce strain
## Reasons I built this
 - Right now, I type on a laptop keyboard and am scared that I might get carpal tunnel.
 - The switches on my other keyboard are very loud, and are not the best for me. Hotswap sockets let me customize the feel.
 - The keyboard doesn't have backlighting.
## Schematic
 For the schematic, I used hierarchial sheets to organize everything. There are 2 hierarchial sheets for each side of the pcb, and a hierarchial sheet in each one of those for the large neopixel matrix. 

 - ![Schematic](assets/schematic.png)
 - ![Neopixels](assets/neopixelmatri.png)
 - ![FullFull](assets/Screenshot%202026-06-06%20at%207.33.07 PM.png)
## PCB
 I designed the PCB with mousebites to make the split keyboard easy to manufacture. I thought of making a reversible PCB at first, but it would be very difficult with an OLED. 
  ### Left side of the PCB 
  ![Left](assets/halfpcb.png)
  ### Full PCB
  ![Full](assets/fullpcb.png)
  ### 3D View
  ![3D](assets/pcb3dview.png)
## CAD
 I designed the CAD with ease of assembly in mind. That is why I designed it with no tolerances, so that it could completely friction fit(I added screw holes for the worst case). I decided to print it with an extra fine setting on my Bambu Lab A1 Mini 3D printer, and it turned out great. 
 ### Bottom Case
 ![Bottom](assets/Bottom.png)
 ### Top Plate
 ![Plate](assets/plate.png)
 ### Full Assembly
 ![Assembly](assets/Assembly.png)
 ### Pictures of it Assembled
 ![Assembly](assets/IMG_2330.HEIC)
 ![Assembly](assets/IMG_2331.HEIC)
## My Zine
![zine](assets/zine.png)
Zine is at zine.pdf too
## Assembly Instructions
 - First, obviously fabricate the PCB and solder everything.
 - Next is printing the plate and case.
 - Print with very fine settings as it friction fits, I printed with 0.08 mm High Quality @BBL on my Bambu Labs A1 Mini.
 - Be careful when removing the plate and bottom from the print bed as it could break
 - Obviously print two of each, two plates and two bottom cases
 - Then, go into the Firmware folder, open the submodule, and open Github Actions
 - Click the latest build and download the firmware artifact.
 - Then, plug in a USB cable into the Xiao and hit the reset button 2 times
 - A drive should show up, drop the first file that says settings-reset etc.
 - The drive should disappear, wait about 5 seconds and then do the same thing again
 - Then drop the file that starts with custom21
 - Now disconnect the cable, and it should show up as a BLE device
 - Connect to it then put the PCB into the bottom case
 - Then put the plate on top of it and place the keycaps on top of that to secure it.
 - You're good to go!
## Credits
 This project is inspired by the Corneucopia project by @DynamicWhiteHat.
 It used Autodesk Fusion for CAD, Kicad 10 for the PCB, and is sponsored by Hack Club Fallout! Thanks to Hack Club for sponsoring this!
