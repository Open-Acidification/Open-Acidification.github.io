---
title: Device Assembly
---

## 3D printing of housing
Coming Soon


## Prepare Housing

1. Remove 3-d extra printing
1. Insert press nuts

## Solder header pins to LCD module

Solder the 16-pin male header to the LCD module on the opposite face of the module from LCD screen. It often help to stick the header pins into a breadboard and then place the LCD module over the headers on the breadboard.

![Parts for the LCD screen](/assets/images/lcd_parts.jpg)
![LCD screen with male header soldered](/assets/images/lcd_soldered.jpg)

## Assemble Faceplate

Parts needed:
* 3D printed faceplate
* LCD module
* 2x 6-pin female-male jumper cables
* 4x4 matrix keypad
* Button
* 2x 20cm solid core 22 AWG wire
* 4x M3 x 0.5 Socket hex head bolts
* 4x M3 nuts
* Metric 2.5 alan wrench
* 5.5 mm socket wrench

![Parts needed to assemble the faceplate](/assets/images/faceplate_parts.jpg)

### Attaching reset button

Cut two sections of solid core 14 gauge wire to 20cm.  Strip the insulation from ~1cm from each end of each wire.

![Stripped wired for reset button](/assets/images/reset_wires.jpg)

Next, solder one end of each wire to the terminals of the reset button.

![A reset wire soldered to one of the terminals of the reset button](/assets/images/reset_solder.jpg)

Disassemble the button pulling the red button cap from the button pin.  Then, unscrew the nut from the button.

![Reset button disassembled and ready to attach to the faceplate](/assets/images/reset_disassemble.jpg)

Place the hex nut into the the hexagonal pocket in the faceplate above the "RESET" text.

![Reset button nut set into the hexagonal pocket](/assets/images/reset_nut.jpg)

Now, push the reset button through the back face of the faceplate and screw it into the nut until the button assembly is tight against the faceplate.

![Reset button threaded into the nut on the faceplate](/assets/images/reset_thread.jpg)
![Reset button seated against the faceplate](/assets/images/reset_screwed.jpg)

Finally, reseat the red button cap onto the pin.

### Attach keypad to faceplate

![Keypad and faceplate](/assets/images/keypad_faceplate.jpg)

First, peel the paper backing from the keypad.
![Peeling the paper bacing from the keypad](/assets/images/keypad_peel.jpg)

Then, carefully place the female header and flex cable through the slot in the lower portion of the faceplate.
![Threading flex cable through the slot in the faceplate](/assets/images/keypad_insert.jpg)

Pull the flex cable through from the back side of the faceplate to take up the clas in the cable with one hand while placing the keypad square (so the bottom edge is parallel with the bottom edge of the faceplate) with the other hand. Once the keypad is placed down on the faceplate, press down firmly on all parts of the keypad to securely adhere the keypad to the faceplate.
![Placing the keypad onto the faceplate](/assets/images/keypad_stick.jpg)

### Attach LCD screen to faceplate

![LCD and faceplate](/assets/images/lcd_faceplate.jpg)

Place the LCD module into the large opening in the top portion of the faceplate from the backside of the faceplate.
![Positioning the LCD in the faceplate](/assets/images/lcd_placement.jpg)

Then, place bolts through each of the four holes through the LCD and faceplate at the corners of the LCD module. Tighten nuts with the alan wrench and socket wrench.
![Bolting LCD to the faceplate](/assets/images/lcd_bolt.jpg)

Finally, place female/male jumper cables on the 6 pins on each end of the header pins on the LCD module.
![Jumper cables placed on the LCD module](/assets/images/lcd_jumpers.jpg)

## Preparing electrical outlets

Parts & Tools needed:
* 14 gauge stranded wire (three colors: white, green and red)
  * one 15 cm section in each color
  * one 10 cm section in each color
* 2x panel mount power receptacle
* Strippers
* Soldering Iron
* Helping hands

First, strip 0.5-1 cm of insulation from the end of each section of wire
![Tools needed to prepare electrical outlets](/assets/images/outlet_stripped.jpg)

Next, using the helping hands, solder the 15 cm wires to the tabs on one of the power receptacle.  
![Using helping hands to solder wires to the electrical outlets](/assets/images/outlet_helping_hands.jpg)

The red wire should be attached to the upper left tab (as you are looking at the tabs straight on), sometimes marked "LM", the white to the upper left tab, sometimes marked "W", and the green wire to the lower tab, sometimes also marked "G". The tin the opposite end with the wires with solder.
![Wires soldered to the electrical outlets](/assets/images/outlet_soldered.jpg)

Repeat this process with the 10 cm wires and the other power receptacle. Set these aside for later.
![Finished electrical outlets](/assets/images/outlets_finished.jpg)

## Preparing Housing Skirt

Parts and Tools needed:
* 8x M4 Press-Fit nuts
* At least 1 M4 bolt
* 3D printed housing skirt
* Either 3D printed faceplace or backplate

Place one of the push nuts into the holes in the corners of housing skirt.  It will likely not be possible to sink the push nut into the hole by pushing alone.
![Initial placement of push nut](/assets/images/pushnut_placement.jpg)

Because it is generally not possible to push in the nuts with one's hands, I generally use a bolt to accomplish this.  To to this, hold the nut in place with one hand, turn the skirt over and one of the countersunk holes in either the faceplate or the backplate over the hole in which the push nut has been place. Then place a bolt through through that hole and thread it into the push nut.
![Bolt placement to sink push nut into hole](/assets/images/pushnut_screw.jpg)
![Bolt threaded through push nut](/assets/images/pushnut_threaded.jpg)

Finally, screw the bolt down to pull the push nut into the hole until the exposed face is flush with the plastic. Repeat in the other seven corner of the skirt.
![Push nut sunk into hole](/assets/images/pushnut_sunk.jpg)


## Final Device Assembly

Parts and Tools needed:
* Prepared housing skirt
* Prepared electrical receptacles
* Arduino Mega 2560
* Arduino Ethernet Shield v1 (Wiznet 5100)
* Assembled PCB
* Assembled faceplate
* backplate

![Parts for final device assembly](/assets/images/final_assembly.jpg)

Plug the Ethernet Shield into the Aruino Mega
![Ethernet Sheild attached to Arduino Mega](/assets/images/ethernet_shield.jpg)
