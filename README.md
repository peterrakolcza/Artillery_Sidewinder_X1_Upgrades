# Artillery Sidewinder X1 🖨️


<img align="right" width="175" src="https://github.com/MarlinFirmware/Marlin/raw/2.0.x/buildroot/share/pixmaps/logo/marlin-250.png" style="max-width:100%;">

<img align="left" width="175" src="https://github.com/pinguinpfleger/ASWX1-FW-MOD/blob/2.0.x/artillery_logo_brand.png?raw=true" style="max-width:100%;">

 
The present repository is dedicated to optimizing the Artillery Sidewinder X1 3D printer. If you're in search of enhancements to apply to your Sidewinder X1, you've landed on the right page. Within this repository, I'll be sharing my recommended upgrades for the Sidewinder X1. This information should streamline your decision-making process when considering modifications for your Sidewinder X1.

While many acknowledge the Sidewinder X1 as a proficient machine in its original setup, there will always be enthusiasts seeking to maximize their printer's performance.

I partially concur that the X1 operates effectively in its standard configuration. My Artillery Genius (the X1’s counterpart) currently operates with its default settings and produces impressive prints. However, I opted to enhance the X1 to address minor issues I encountered and to compile guides and tutorials.

<br>
   
## 🚀 Upgrades

- [Small upgrades](#small-upgrades)
    - [Aluminum Extruder Idler Lever](#aluminum-extruder-idler-lever)
    - [Gantry Support](#gantry-support)
    - [Squaring the Gantry](#squaring-the-gantry)
    - [Better Quality Nozzles](#better-quality-nozzles)
    - [Jaw Couplers with Rubber Interface](#jaw-couplers-with-rubber-interface)
    - [POM Anti-Backlash Nuts](#pom-anti-backlash-nuts)
    - [Bi-Metal Heatbreak](#bi-metal-heatbreak)
- [LED Light](#led-light)
- [BLTouch for Auto Bed Leveling](#bltouch-for-auto-bed-leveling)
- [Marlin + TFT Firmware](#marlin--tft-firmware)
- [OctoPi](#octopi)
- [Obico for OctoPrint](#obico)

## 🤏 Small upgrades

### Aluminum Extruder Idler Lever

Description of the upgrade: Replace the stock plastic extruder idler lever with a more durable and efficient aluminum lever for better extrusion performance.

### Gantry Support

Description of the upgrade: Strengthen the printer's gantry system to improve stability and precision during printing.

### Squaring the Gantry

Description of the upgrade: Instructions on how to properly square the gantry for optimal printer performance and print accuracy.

### Better Quality Nozzles

Description of the upgrade: Upgrade to higher-quality nozzles to enhance printing precision and reduce clogs.

### Jaw Couplers with Rubber Interface

Description of the upgrade: Upgrade the jaw couplers to those with a rubber interface to minimize vibrations and improve print quality.

### POM Anti-Backlash Nuts

Description of the upgrade: Replace standard nuts with POM anti-backlash nuts for smoother and more precise movements.

### Bi-Metal Heatbreak

Description of the upgrade: Replace the heatbreak with a bi-metal version for improved heat dissipation and reduced heat creep.

## 💡 LED Light

Description of the upgrade: Install LED lighting to illuminate the print bed and enhance visibility during printing.

## 💉 BLTouch for Auto Bed Leveling

Description of the upgrade: Implement BLTouch for automated bed leveling, ensuring a level print surface for each print job.

## 🖥️ Marlin + TFT Firmware

Description of the upgrade: Upgrade the printer's firmware to Marlin and integrate a TFT touchscreen for an improved user interface and enhanced control.

## 🐙 OctoPi

Description of the upgrade: Set up OctoPi to remotely monitor and manage the 3D printer, providing convenient access and control.

## 📷 Obico for OctoPrint

Obico is an OctoPrint plugin designed to enhance 3D printing workflows. It provides improved visualizations, analytics, and additional features to optimize your printing experience, making it a valuable tool for managing your 3D printer and prints within the OctoPrint ecosystem.

## 🛠️ Compatibility and Usage with OctoPrint

The serial bus with the main board (MKS GEN L v1.0) is shared between TFT and Octoprint / Pronterface etc… This means that printing from Octoprint / Pronterface etc… causes Marlin to receive gcodes from Octoprint and TFT at the same time (there are collisions). This will let Marlin reply with error messages, that will be displayed on both Octoprint and TFT display, such as:

```
Line Number is Not Last Line Number +1 Last Line 1686.
```

In order to avoid the problem, when printing with Octoprint/Pronterface etc… put the TFT in “Listening Mode” pressing on the button:
``` 
Menu => Settings => Connection => ON
```

### 📌 Note:

- This limitation is not due to bugs on the TFT firmware but it is an hardware limitation on MKS GEN L v1.0 main board
- The mode state is stored on FLASH allowing to restore the mode at startup. This allows to power on/off the printer remotely and to control the printer via USB without the need of any touch (from the user) on the display to engage the mode


## 📚 References
- [Artillery Sidewinder X1 Upgrades – Paid and Free](https://3dprintbeginner.com/sidewinder-x1-upgrades/)
- [Artillery Sidewinder X1 / X2 / Genius TFT FW + Marlin FW (for X1) + M600 support + Marlin mode …](https://3dfablab.wordpress.com/2021/12/07/artillery-sidewinder-x1-x2-genius-tft-fw-marlin-fw-for-x1-m600-support-marlin-mode/)
- [Self-hosted Obico Server Guides](https://www.obico.io/docs/server-guides/)
- [BLTouch for Auto Bed Leveling](https://www.youtube.com/watch?v=1uuxTWJZowo) 
- [Sidewinder X1 Gantry Support](https://www.youtube.com/watch?v=9TPCdesemes) 
- [Squaring the gantry on the Sidewinder X1 3D printer, the EASY way.](https://www.youtube.com/watch?v=KmeYlX6eXGE)