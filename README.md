# Artillery Sidewinder X1 🖨️


<img align="right" width="175" src="https://github.com/MarlinFirmware/Marlin/raw/2.0.x/buildroot/share/pixmaps/logo/marlin-250.png" style="max-width:100%;">

<img align="left" width="175" src="https://github.com/pinguinpfleger/ASWX1-FW-MOD/blob/2.0.x/artillery_logo_brand.png?raw=true" style="max-width:100%;">

 
The present repository is dedicated to optimizing the Artillery Sidewinder X1 3D printer. If you're in search of enhancements to apply to your Sidewinder X1, you've landed on the right page. Within this repository, I'll be sharing my recommended upgrades for the Sidewinder X1. This information should streamline your decision-making process when considering modifications for your Sidewinder X1.

While many acknowledge the Sidewinder X1 as a proficient machine in its original setup, there will always be enthusiasts seeking to maximize their printer's performance.

I partially concur that the X1 operates effectively in its standard configuration. My Artillery Genius (the X1’s counterpart) currently operates with its default settings and produces impressive prints. However, I opted to enhance the X1 to address minor issues I encountered and to compile guides and tutorials.

<br>
   
## 🚀 Upgrades

- [Small upgrades](#-small-upgrades)
    - [Aluminum Extruder Idler Lever](#aluminum-extruder-idler-lever)
    - [Gantry Support](#gantry-support)
    - [Squaring the Gantry](#squaring-the-gantry)
    - [Better Quality Nozzles](#better-quality-nozzles)
    - [Jaw Couplers with Rubber Interface](#jaw-couplers-with-rubber-interface)
    - [POM Anti-Backlash Nuts](#pom-anti-backlash-nuts)
    - [Bi-Metal Heatbreak](#bi-metal-heatbreak)
- [LED Light](#-led-light)
- [BLTouch for Auto Bed Leveling](#-bltouch-for-auto-bed-leveling)
- [Marlin + TFT Firmware](#-marlin--tft-firmware)
- [OctoPi](#-octopi)
- [Obico for OctoPrint](#-obico-for-octoprint)

## 🤏 Small upgrades

You can find detailed explanations and recommended parts about each upgrade on this website ([Artillery Sidewinder X1 Upgrades – Paid and Free](https://3dprintbeginner.com/sidewinder-x1-upgrades/)).

### Aluminum Extruder Idler Lever

Replace the stock plastic extruder idler lever with a more durable and efficient aluminum lever for better extrusion performance.

### Gantry Support

Strengthen the printer's gantry system to improve stability and precision during printing. STL files are included in the repository.
[Video Tutorial](https://www.youtube.com/watch?v=9TPCdesemes) 

### Squaring the Gantry

Instructions on how to properly square the gantry for optimal printer performance and print accuracy. STL files are included in the repository.
[Video Tutorial](https://www.youtube.com/watch?v=KmeYlX6eXGE)

### Better Quality Nozzles

Upgrade to higher-quality nozzles to enhance printing precision and reduce clogs.

### Jaw Couplers with Rubber Interface

Upgrade the jaw couplers to those with a rubber interface to minimize vibrations and improve print quality.

### POM Anti-Backlash Nuts

Replace standard nuts with POM anti-backlash nuts for smoother and more precise movements.

### Bi-Metal Heatbreak

Replace the heatbreak with a bi-metal version for improved heat dissipation and reduced heat creep.

## 💡 LED Light

Install LED lighting to illuminate the print bed and enhance visibility during printing. I just added a 24V led strip to the power supply and routed the cable through the gantry.

![24V LED](/images/IMG_0174.jpg)

## 💉 BLTouch for Auto Bed Leveling

The Sidewinder X1 is a 3D printer known for its large print volume and reliability. The BLTouch is an auto-bed leveling sensor commonly used in 3D printers to help achieve a level print bed, which is crucial for successful 3D prints. Installing a BLTouch on the Sidewinder X1 can greatly improve the quality of your prints by ensuring the first layer adheres well to the bed and is consistent across the entire print surface.

There is a great video tutorial ([Youtube Tutorial](https://www.youtube.com/watch?v=n8kRF9XfeNo)) showing the whole process, but here are the general steps to install a BLTouch on a Sidewinder X1:

1. Gather the Required Components:
    - BLTouch auto-bed leveling sensor
    - Mounting bracket for the BLTouch (you may need to 3D print)
    - Wires and connectors for connecting the BLTouch to the printer's electronics (usually comes with the BLTouch)

2. Print or Acquire a Mounting Bracket:
    - Print or acquire a suitable mounting bracket for the BLTouch that is compatible with the Sidewinder X1's frame and hotend assembly.

3. Install the Mounting Bracket:
    - Attach the mounting bracket to the hotend assembly of the Sidewinder X1. Ensure that the BLTouch sensor will be positioned accurately and at an appropriate height above the print bed.

4. Wire Connection:
    - Connect the BLTouch to the appropriate pins on the control board of the Sidewinder X1. You'll need to connect the necessary wires for power, ground, and signal.
    - It is recommended to use the built-in LED on the extruder for easy installation.

5. Firmware Configuration:
    - Modify the firmware of the 3D printer to accommodate the BLTouch sensor. You will need to enable the BLTouch feature in the firmware and configure the sensor's settings, such as offsets and probe points.
    - Refer to [Marlin + TFT Firmware](#marlin--tft-firmware).

6. Calibration:
    - Use the printer's firmware interface to calibrate the BLTouch. This involves adjusting the probe offsets, homing the printer, and fine-tuning the Z-offset to ensure the nozzle is at the correct height above the bed.

After finishing everything the connection to the main board should look like this:

![Main board wiring](/images/IMG_0178.jpg)

## 🖥️ Marlin + TFT Firmware

Upgrade the printer's firmware to Marlin and integrate a TFT touchscreen for an improved user interface and enhanced control. Use the included firmware in the repository for the main board (aswx1_marlin_fw_2.1.2_bltouch_waggster_mod_z_max_used.rar) and TFT panel (artillery_tft_fw_1.27.x_patch_9.5.rar).


## 🐙 OctoPi

OctoPi (OctoPrint on Raspberry Pi) is a popular open-source software that allows you to remotely monitor and control your 3D printer through a web interface. Setting up OctoPi with the Sidewinder X1 allows you to have a more convenient and remote way to manage your 3D prints. Here are the steps to set up OctoPi with the Sidewinder X1:

1. Obtain a Raspberry Pi:
Obtain a Raspberry Pi (e.g., Raspberry Pi 4) and a suitable microSD card (16GB or larger). Install the latest version of OctoPi on the microSD card.

2. Connect the Raspberry Pi:
Insert the microSD card into the Raspberry Pi, connect the Raspberry Pi to your local network using an Ethernet cable or Wi-Fi, and power it up.

3. Access OctoPrint Interface:
On a computer connected to the same network, open a web browser and enter the IP address of your Raspberry Pi or "http://octopi.local" (if Bonjour is supported on your network). The OctoPrint interface should load.

4. Initial Setup:
Follow the on-screen instructions to complete the initial setup, including creating a username and password.

5. Connect Sidewinder X1 to OctoPrint:
Connect the Sidewinder X1 to the Raspberry Pi using a USB cable. The USB cable should be plugged into the Raspberry Pi's USB port.

6. Configure OctoPrint:
In OctoPrint's settings, configure the printer profile for the Sidewinder X1, including the bed size, print volume, and other relevant settings.

7. Test Connection:
Verify that OctoPrint is communicating with the Sidewinder X1 by homing the printer and sending manual movement commands.

8. Install Plugins (Optional):
Customize OctoPrint by installing plugins that enhance its functionality, such as plugins for temperature monitoring, timelapse recording, and more.

9. Remote Monitoring and Control:
Use OctoPrint's web interface to remotely monitor and control your Sidewinder X1. You can start, pause, and stop prints, monitor print progress, and even receive notifications.

10. Secure Access (Optional):
Consider securing your OctoPrint instance by enabling access control, using HTTPS, and configuring firewall rules to restrict access to trusted IP addresses. Refer to [Obico for OctoPrint](#-obico-for-octoprint).

Sample wiring inside of the Sidewinder X1 for a cleaner look:

![Main board wiring](/images/IMG_0175.jpg)

### 🛠️ Compatibility and Usage with OctoPrint

The serial bus with the main board (MKS GEN L v1.0) is shared between TFT and Octoprint / Pronterface etc… This means that printing from Octoprint / Pronterface etc… causes Marlin to receive gcodes from Octoprint and TFT at the same time (there are collisions). This will let Marlin reply with error messages, that will be displayed on both Octoprint and TFT display, such as:

```
Line Number is Not Last Line Number +1 Last Line 1686.
```

In order to avoid the problem, when printing with Octoprint/Pronterface etc… put the TFT in “Listening Mode” pressing on the button:
``` 
Menu => Settings => Connection => ON
```

#### 📌 Note:

- This limitation is not due to bugs on the TFT firmware but it is an hardware limitation on MKS GEN L v1.0 main board
- The mode state is stored on FLASH allowing to restore the mode at startup. This allows to power on/off the printer remotely and to control the printer via USB without the need of any touch (from the user) on the display to engage the mode

### 🛠️ Printing from Remote Host

After the TFT is set to Listening Mode (see section Integration with OctoPrint),

OctoPrint, ESP3D, Pronterface etc, connected to a TFT's or mainboard's serial port, can host a print (print handled by the host) and optionally can trigger some actions to the TFT sending specific G-codes. Refer to the documentation.

### 🛠️ Filament Sensor with OctoPi

Adding the filament sensor to your OctoPi for remote monitoring and control, is a great way to enhance your 3D printing experience. A filament sensor can help you avoid failed prints due to filament runouts. As it is connected to the TFT panel, it cannot be used directly when printing from remote host (OctoPi).

However, you can wire it to the GPIO pins on the OctoPi and use the *Filament Sensor Simplified* plugin. **Note: you will not able to use the filament sensor when printing from USB or SD card!**

I used toothpicks to get out the crimpled wires from the connectors and use new connectors. If you are using the same power supply for the OctoPi as for your main board, then you can leave the 3.3V and GND wires in-place and connect the sensor wire to GPIO24 (as they share the common ground). Otherwise, you have to wire everything into the OctoPi (as I did). Refer to the pictures for wiring, I have used 3.3V, GND and GPIO24 pins on the OctoPi.

![Wiring 1](/images/IMG_0187.jpg)
![Wiring 2](/images/IMG_0188.jpg)

## 📷 Obico for OctoPrint

Obico is an OctoPrint plugin designed to enhance 3D printing workflows. It provides improved visualizations, analytics, and additional features to optimize your printing experience, making it a valuable tool for managing your 3D printer and prints within the OctoPrint ecosystem.

I am recommending to use a self-hosted server as it makes the whole setup free. Refer to [Self-hosted Obico Server Guides](https://www.obico.io/docs/server-guides/) for a more detailed guide.


## 📚 References
- [Artillery Sidewinder X1 Upgrades – Paid and Free](https://3dprintbeginner.com/sidewinder-x1-upgrades/)
- [Artillery Sidewinder X1 / X2 / Genius TFT FW + Marlin FW (for X1) + M600 support + Marlin mode …](https://3dfablab.wordpress.com/2021/12/07/artillery-sidewinder-x1-x2-genius-tft-fw-marlin-fw-for-x1-m600-support-marlin-mode/)
- [Self-hosted Obico Server Guides](https://www.obico.io/docs/server-guides/)
- [BLTouch for Auto Bed Leveling](https://www.youtube.com/watch?v=1uuxTWJZowo) 
- [Sidewinder X1 Gantry Support](https://www.youtube.com/watch?v=9TPCdesemes) 
- [Squaring the gantry on the Sidewinder X1 3D printer, the EASY way.](https://www.youtube.com/watch?v=KmeYlX6eXGE)