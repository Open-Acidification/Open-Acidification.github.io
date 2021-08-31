---
title: Device Software
---

## Software Menus

Because of the limitations of our input and output devices (a 4x4 keypad and a 16x2 LCD), the user interface is designed to be relatively simple. The initial (or _idle_) screen shows the current values and targets for pH and temperature. From this screen you can select a menu to view settings or a menu to change settings.

### Top-level Menu

The idle screen is the first of three top-level screens:

* Idle
* View Settings
* Change Settings

These three screens are connected as a loop where the '2' key goes up and the '8' key goes down. So pressing '8' (down) from the idle screen will take you to the View Settings screen with the following display:

```text
View settings
<4   ^2  v8   6>
```

Note the "^2" for "up" and the "v8" for "down". This is a reminder of how to go up and down through the top-level menu screens. From here, pressing '2' will go "up" to the idle screen and pressing '8' will take you "down" to the Change Settings screen with the following display:

```text
Change settings
<4   ^2  v8   6>
```

From here pressing '2' will go "up" to the View Settings screen and pressing '8' will take you "down" and loop back to the top to show the idle screen.

### View Settings Menu

When on a menu option you can select it by pressing '6' (right). In the case of the "View settings" menu, you will be taken to a new sequence of menus:

* View time
* View PID
* View pH slope
* View tank ID
* View log file
* View Google mins
* View IP and MAC
* View version
* View free memory

As with the top-level menu, you can move down (8) and up (2) and you can select an item (6).
In addition, you can return to the top-level menu by pressing '4' (left).
Selecting a menu item (6>) will take you to the state where you are viewing the requested information.
In most cases you can exit from this state by pressing any key.
If you don't press a key then after a minute the device returns to the idle screen.

### Change Settings Menu

You can select the Change Settings menu by pressing '6' (right) and be taken to a new set of menu options:

* Set pH target
* Set temperature
* pH calibration
* Clear pH calibration
* Temp calibration
* Set KP
* Set KI
* Set KD
* PID on/off
* Set chill/heat
* Set Google mins
* Set date/time
* Set Tank ID

As before, you can move up (2), down (8), left (4), and right (6).
