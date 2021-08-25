---
title: Install Software
---

## Software Installation

The following steps are required to install the TankController software.

1. _Install the [Arduino Desktop IDE](https://www.arduino.cc/en/software)._
    1. Download and unzip the appropriate executable for your platform (Linux, macOS, or Windows; on Windows use the zip file rather than the Windows Store option so that you can edit the config in step 2).
    2. Copy the directory or package to an appropriate place for applications on your platform.
    3. Follow the [Getting Started Guide](https://www.arduino.cc/en/Guide/ArduinoMega2560) to confirm that you can install and run the "Blink" software.

2. _Configure the IDE._ By default, the Arduino compiler links to a `printf()` library that does not support printing floating point numbers (for details see [here](https://forum.arduino.cc/t/no-sprintf-float-formatting-come-back-five-year/331790/6)). To get that feature do the following:
    1. Locate the `boards.txt` file. This file is in the downloaded at `arduino-1.8.15/hardware/arduino/avr/boards.txt` (on macOS look in `~/Library/Arduino15/packages/arduino/hardware/avr/1.8.3`).
    2. Open `boards.txt` in a text editor and look for a `mega.menu` label.
    3. After the existing menu definitions, add the following lines and save the file (take care that your web browser is wide enough so that the lines do not wrap):

```text
## Arduino Mega printf() library options
## -------------------------
menu.printf=AVR printf Version

mega.menu.printf.default=Default printf
mega.menu.printf.default.compiler.c.elf.extra_flags=
mega.menu.printf.full=Full printf
mega.menu.printf.full.compiler.c.elf.extra_flags=-Wl,-u,vfprintf -lprintf_flt
mega.menu.printf.minimal=Minimal printf
mega.menu.printf.minimal.compiler.c.elf.extra_flags=-Wl,-u,vfprintf -lprintf_min
```

3. Launch the Arduino Desktop IDE and use the Tools menu to select `ARV printf Version: "Full printf"`:

![IDE Tools Menu](/assets/images/IDE_tools_menu.jpg)

### TankController software

4. _Download TankController._
    1. Download a [zip](https://github.com/Open-Acidification/TankController/releases) of the [TankController](https://github.com/Open-Acidification/TankController) software.
    2. From the Arduino IDE, follow the instructions on [Importing a .zip Library](https://www.arduino.cc/en/guide/libraries) to install the library.

5. _Install TankController._
    1. In the Arduino Desktop IDE, open `TankController/examples/TankController.ino`.
    2. If you have a PushingBox Identifier, add it where indicated (line 7).
    3. Click the "Upload" button (a right-facing arrow) or select the "Sketch / Upload" menu.
    4. If you do not have an Ethernet cable attached you can shorten the startup time by pressing any key to skip the DHCP request; release the key when you see the idle screen (with current values and targets for pH and temperature).

