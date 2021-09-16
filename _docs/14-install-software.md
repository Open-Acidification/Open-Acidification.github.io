---
title: Install Software
---

## Software Installation

The following steps are required to install the TankController software.

1. _Install the [Arduino Desktop IDE](https://www.arduino.cc/en/software)._
    1. Download and unzip the appropriate executable for your platform (Linux, macOS, or Windows; on Windows use the zip file rather than the Windows Store option so that you can edit the config in step 2).
    2. Copy the directory or package to an appropriate place for applications on your platform.
    3. Follow the [Getting Started Guide](https://www.arduino.cc/en/Guide/ArduinoMega2560) to confirm that you can install and run the "Blink" software.

2. _Download TankController to your computer._
    1. From the Arduino IDE select the menu command `Tools -> Manage Libraries`.
    2. Search for `TankController`, click the `Install` button, and close the Library Manager.

3. _Install TankController to the device._
    1. From the Arduino IDE select the menu command `File -> Examples -> TankController -> TankController`.
    2. If you have a PushingBox Identifier (to send data to the cloud periodically), add it where indicated on line 7.
    3. Click the "Upload" button (a right-facing arrow) or select the "Sketch / Upload" menu.
    4. If you do not have an Ethernet cable attached you can shorten the startup time by pressing any key to skip the DHCP request; release the key when you see the idle screen (with current values and targets for pH and temperature).
