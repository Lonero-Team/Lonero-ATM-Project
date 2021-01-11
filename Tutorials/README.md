## The Lonero ATM Project ~ Tutorial
Being built!

Archived instructions....

[Step 1](https://archive.vn/wip/QjAo4) | [Step 2](https://archive.vn/wip/oicTY) | [Step 3](https://archive.vn/wip/xF90d) | [Step 4](https://archive.vn/wip/Qr4cH) | [Step 5](https://archive.vn/wip/XKHhy) | [Step 6](https://archive.vn/wip/FpZW3) | [Step 7](https://archive.vn/wip/yRiOx) | [Step 8](https://archive.vn/wip/siBF1)


### Step 1
Step 1: is the faceplate (which is optional). One can also make a custom case, 3D printed case, or something w/ a CNC machine. The sky is the limit for really creative and well designed enclosures.
<p align="center">
<img src="https://openbitcoinatm.files.wordpress.com/2014/02/obcatm_faceplate.png" width="550">
</p>
Following this design template of a 12"*12" aluminum piece of metal, make the rectangular cuts. Drill the six rivet holes and four holes seen on the template. This will help with attaching the bill acceptor.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/holesvw.png">
</p>

If you were to make the case; \
Cut two aluminum angles into 11 1/2″ lengths (as per original instructions). \
Drill/[tap](https://en.wikipedia.org/wiki/Tap_and_die#mediaviewer/File:Tap_and_T-wrench.jpg) two holes, and drill three rivet holes for the faceplate. (See diagram to avoid confusion).

Remember to rivet the two aluminum angles. You will need to rivet them to the sides of the flaceplate. Make sure to allow for (about 1/8″) room to overlap the surface at the front of the box (as per instructions). The angles should be positioned to lie inside the box.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/fabrivot.png">
</p>

Next, you are going to have to drill 4 holes in the acrylic case (if you decide to use an acrylic case) to match with the metal frame. Please make sure to use an acrylic bit, or  drill slowly.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/plugbarrel.png">
</p>

The next part is if you go with the acrylic case, (or have a difference case), is to solder a barrel plug. This will be done w/ 16" leads that can be soldered to the barrel plug and J2 connectors. One can put PVC tape to hold the wires in place.

### Step 2
The next step is to attach the bill acceptor and printer. You can use zip ties or four screws, washers and nuts.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/acceptorprinter.png">
</p>

### Step 3
The next step is to start setting up the *Arduino UNO*. First, download the [IDE](https://create.arduino.cc/) for Arduino. You can use either the cloud or web editor. Use the [IDE](https://create.arduino.cc/) to upload the [openloneroatm.ino](https://github.com/Lonero-Team/Lonero-ATM-Project/blob/main/OpenATM%20Files/openloneroatm.ino) file to the Arduino.

### Step 4
The next step is to solder the resistor and leads to the SD shield per the circuit diagram.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/SDShield.png">
</p>
<p align="center">
<img src="https://content.instructables.com/ORIG/FMA/9Q3M/HVTWBLCH/FMA9Q3MHVTWBLCH.png" width="550">
</p>

### Step 5
Step 5 involves attaching the components.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/UNOSDShield.png">
</p>

Once you attach the SD shield to the Arduino, mount the Arduino to the "faceplate" of your case design. Connect the J2 connectors and rest of the components as  per the circuit design. Make sure to include a 5V power supply for rechargeability capability.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/faceplatecompnt.png">
</p>

### Step 6
The next step is to create preconfigured private keys for [Lonero](https://lonero.org). Once you create [Lonero](https://lonero.org) private keys, follow these instructions:
1. Download this repo
2. `cd` into `QRCode Maker/` and run the `LNRQRMaker.html` file.
3. Create QR codes for the private  keys
4. Copy the `logo.oba` [file](https://github.com/Lonero-Team/Lonero-ATM-Project/blob/main/OpenATM%20Files/logo.oba) into the root directory of the SD card.

For the naming conventions, make sure that each QR codoe is renamed with the naming convention `LNR_1.lnr`, `LNR_2.lnr`, etc. in the SD card's root directory.

### Step 7
Now you need to work on configuring the bill acceptor.

<p align="center">
<img src="https://raw.githubusercontent.com/Mentors4EDU/Images/master/config_bill_acceptor.PNG">
</p>
<p align="center">
| Configuration Card sample |
</p>

Next, you'll need to print the configuration card for your bill acceptor. The manual includes a configuration card. Fill in the ovals in the configuration card example w/ dark circles.

Hold the reset button for > 10 seconds. When the lights start blinking, feed the configuration card to the bill acceptor's slot. The acceptor will reject it and then rapidly blinked if it was configured correctly.
