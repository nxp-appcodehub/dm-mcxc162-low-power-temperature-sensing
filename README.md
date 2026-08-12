# NXP Application Code Hub
[<img src="https://mcuxpresso.nxp.com/static/icon/nxp-logo-color.svg" width="100"/>](https://www.nxp.com)

## MCXC162 Low Power Temperature Sensing

This demo presents the low power temperature sensing on FRDM‑MCXC162 platform using an onboard P3T1755 temperature sensor. The application spends most of its time in a low-power state. When the wakeup button is pressed. presence is detected, the MCU transitions to active mode, reads the sensor measurement data,and print through serial port.


The P3T1755 is a temperature-to-digital converter from -40 °C to +125 °C range. It uses an on-chip band gap temperature sensor and A-to-D conversion technique with an overtemperature detection. The device contains a number of configuration and data registers to store the device settings, such as device operation mode, and a temperature register (Temp) to store the digital temp reading that can be communicated by a controller via the 2-wire serial I3C (up to 12.5 MHz) and I2C (up to 3.4 MHz) interface.



#### Boards: FRDM-MCXC162
#### Categories: Low Power
#### Peripherals: I2C
#### Toolchains: MCUXpresso IDE, VS code

## Table of Contents
1. [Software](#step1)
2. [Hardware](#step2)
3. [Setup](#step3)
4. [Results](#step4)
5. [FAQs](#step5) 
6. [Support](#step6)
7. [Release Notes](#step7)

## 1. Software<a name="step1"></a>
- Download and install [MCUXpresso IDE V25.06 or later](https://www.nxp.com/design/design-center/software/development-software/mcuxpresso-software-and-tools-/mcuxpresso-integrated-development-environment-ide:MCUXpresso-IDE).
- Download MCU SDK:[SDK_26_06_00_FRDM-MCXC162](https://mcuxpresso.nxp.com/en/welcome)
- Download the code from Git repository dm-mcxc162-low-power-presence-detection<!--[dm-mcxc162-low-power-presence-detection](https://github.com/nxp-appcodehub/dm-mcxc162-low-power-presence-detection)-->.  
- MCUXpresso for Visual Studio Code: This example supports MCUXpresso for Visual Studio Code, for more information about how to use Visual Studio Code please refer [here](https://www.nxp.com/design/training/getting-started-with-mcuxpresso-for-visual-studio-code:TIP-GETTING-STARTED-WITH-MCUXPRESSO-FOR-VS-CODE).

## 2. Hardware<a name="step2"></a>
- FRDM-MCXC162
- USB Type-C cable

## 3. Setup<a name="step3"></a>
### 3.1 Import project from Application Code Hub
1. Open VS code, open MCUXpresso for VSCode extension.
2. In Quick Start Panel window click in Application Code Hub.
[<p align="left"><img src="./picture/vscode_ach.png" width="400"/></p>]()
3. In Search text field, type the name of this example "MCXC162 Low Power Temperature Sensing
4. Select the example, update the name and select the directory where the example will be saved.
5. Click on the import project and wait some minutes.
6. Add the toolchain: Arm GNU
7. Now, the projects of demo should be in projects panel.
8. Now you should have the “dm-mcxc162-low-power-temperature-sensing” in your workspace.

### 3.2 Prepare FRDM and Shield boards
1. Connect FRDM board to computer with USB-C cable in MCU-Link port of FRDM.
2. Open MCUXpresso extension in VSCode.
3. Select the project "dm-mcxc162-low-power-temperature-sensing".
4. Do right click on project and select pristine build and wait about a one minute.
5. Click run (play icon).
6. Please wait a few seconds.
7. Now click stop in center upper button.

## 4. Results<a name="step4"></a>
If you click SW2, the MCU will wake up from low power mode to active mode. The debug console will  print its measured temperature.Then it will sleep.

[<p align="left"><img src="./picture/result.png" width="400"/></p>](./picture/result.png)



#### Project Metadata

<!----- Boards ----->
[![Board badge](https://img.shields.io/badge/Board-FRDM&ndash;MCXC162-blue)]()

<!----- Categories ----->
[![Category badge](https://img.shields.io/badge/Category-LOW%20POWER-yellowgreen)](https://mcuxpresso.nxp.com/appcodehub?category=low_power)

<!----- Peripherals ----->
[![Peripheral badge](https://img.shields.io/badge/Peripheral-I2C-yellow)](https://mcuxpresso.nxp.com/appcodehub?peripheral=i2c)

<!----- Toolchains ----->
[![Toolchain badge](https://img.shields.io/badge/Toolchain-MCUXPRESSO%20IDE-orange)](https://mcuxpresso.nxp.com/appcodehub?toolchain=mcux)
[![Toolchain badge](https://img.shields.io/badge/Toolchain-VS%20CODE-orange)](https://mcuxpresso.nxp.com/appcodehub?toolchain=vscode)

Questions regarding the content/correctness of this example can be entered as Issues within this GitHub repository.

>**Note**: For more general technical questions regarding NXP Microcontrollers and the difference in expected functionality, enter your questions on the [NXP Community Forum](https://community.nxp.com/)

[![Follow us on Youtube](https://img.shields.io/badge/Youtube-Follow%20us%20on%20Youtube-red.svg)](https://www.youtube.com/NXP_Semiconductors)
[![Follow us on LinkedIn](https://img.shields.io/badge/LinkedIn-Follow%20us%20on%20LinkedIn-blue.svg)](https://www.linkedin.com/company/nxp-semiconductors)
[![Follow us on Facebook](https://img.shields.io/badge/Facebook-Follow%20us%20on%20Facebook-blue.svg)](https://www.facebook.com/nxpsemi/)
[![Follow us on Twitter](https://img.shields.io/badge/X-Follow%20us%20on%20X-black.svg)](https://x.com/NXP)

## 5. Release Notes<a name="step7"></a>
| Version | Description / Update                           | Date                        |
|:-------:|------------------------------------------------|----------------------------:|
| 1.0     | Initial release on Application Code Hub        | August 12<sup>th</sup> 2026 |
