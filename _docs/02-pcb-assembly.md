---
title: PCB Assembly
---

## Tools Required

* Soldering iron
* Pliers
* Wire cutters
* Desoldering pump (solder sucker)
* solder
* Breadboard

## Preparatory Steps
### Reverse the direction of pins on 2 relay module

![2-Relay Module Header Pins](/assets/images/relay_headers.jpg)

1. Pull plastic base up and off using a pair of pliers.

![2-Relay Module Header Pins partially removed](/assets/images/Relay_remove_partial.jpg)

  * Tip - If it is difficult to remove the plastic base, cut the base so it only is connect to a single pin. Then pull it off.

![2-relay module without rubber base](/assets/images/plastic_retainer_removed.jpg)

2. Remove pins by grasping the longer end of the pins with a pair of plier and gently pulling away from the board while simultaneously heating the solder with the iron to release the pin.

  ![Removing relay pins](/assets/images/relay_remove_pins.jpg)

  When you have completed this step, the through-holes on the board will likely still be filled with remnant solder.

  ![Remaining solder in through holes](/assets/images/solder_remnant.jpg)

3. Next, remove solder from the through-holes by placing the aperature of the solder sucker directly over a through hole, while simultaneously heating the solder in the through hole with the soldering iron. When the solder liquefies, fire the solder sucker to remove the solder from the hole.  You may need to repeat this step multiple times per through-hole to completely clear the hole of solder.  Be careful not to leave the soldering iron on the through-hole too long and cause the pad to separate form the PCB.  

  ![Clearing through-holes of solder](/assets/images/solder_sucking.jpg)

  ![joint clear of soldier](/assets/images/cleared_through_hole.jpg)

  You may need to remove soldier from both sides.

  You can check by attempting to push the clean end of one of the removed pins through the joint. If you can push the pin through easily, it has been cleared. If it fits through, but tightly, you can spin the spin (which should be square in cross-section) in the hole to clear away the last few bits of solder.

1. Attach new header pins
  Finally, solder on new pins in the reverse orientation.
![Pins reversed on relay module](/assets/images/reversed_pins.jpg)

### Prepare 5V and 9V buck converts

* The bill of materials includes two 16-pin male headers.  One of these we will use to supply single pin male headers. Use pliers or wire cutters to break off eight single male header pins.

![Cutting male headers](/assets/images/cutting_headers.jpg)

![Buck converters and header pins](/assets/images/Buck_converters.jpg)

* Put two single male header pins on a breadboard two positions apart, somewhere towards the middle of the board, then put buck converter on top

![Pin placement](/assets/images/pin_placement.jpg)

![Buck converter placed on top of pins](/assets/images/buck_on_top.jpg)

* Solder those two pins in place

* Place two pins four positions apart on the breadboard 9 rows away from the end of the breadboard (this should allow just enough room for the two pins previously soldered to hang over the edge.).  

![Placement of second pin set](/assets/images/second_pin_placement.jpg)

* Place buck converter on top of these pins.  These pins are very close to a large capacitor that may have to be bent upwards away form the pins in order to safely solder.

![Buck on top of pins again](/assets/images/second_buck_on_top.jpg)

* Repeat with second buck converter.

![Finished buck converter](/assets/images/finsihed_buck_converter.jpg)



## Soldering Arduino Header Pins

![Arduino, 2.5 mm header pins and custom pcb]()

* Arduino Mega
* 2x 2.5 mm 4 header pins
* 1x 2.5 mm 2x18 header pins
* Custom pcb

![Arduino Pins Layed Out](/assets/images/Arduno_Header_Layout.jpg)

![Placed header pins on Arduino]()

![Arduino Pins Placed](/assets/images/Arduino_header_pins_placed.jpg)

![Place PCB on header pins]()

![PCB placed on the Arduino header pins](/assets/images/PCB_on_arduino_header_pins.jpg)

![Soldier pins on PCB]()

![Soldering the first pin into place on Arduino header pins](/assets/images/Solder_Arduino_Header_Pins1.jpg)

![Soldering the first header set into place on Arduino header pins](/assets/images/Solder_Arduino_Header_Pins2.jpg)

![Soldering the other header set into place on Arduino header pins](/assets/images/Arduino_header_soldering.jpg)

![Arduino header pins fully soldered](/assets/images/Arduino_header_soldered.jpg)

Carefully remove PCB from arduino

![PCB removed from Arduino](/assets/images/PCB_removed.jpg)


![Arduino and custom pcb with soldiered header pins]()

## Attaching pH carrier board female header

![Tools needed]()
* 5 position female header for the pH carrier board
* Custom pcb

There are many methods one could use to attach this header. Here we demonstrate how we have done it.
* Fill first through hole with solder (We use a PCB holder or this process)
![image of PCB placed in PCB holder](/assets/images/PCB_holder.jpg)

![Filling first through hole](/assets/images/Fill_first_through_hole.jpg)

![First through hole filled](/assets/images/Filled_Hole.jpg)

* Position the five pins of the header along the five through holes in the box labeled "pH carrier1". Pay attention to the header is on the opposite face of the PCB from the Arduino header pins. Once placed press gently against the pin placed in the filled through hole.

![Pressing header](/assets/images/Gentle_Press.jpg)

* While pressing header pin against filled through hole, heat the other side of the through hole with your soldering iron. Your pin should fall through the hole and become attached to the board.

![heating through hole](/assets/images/heating_through_hole.jpg)

* Now that the first pin is set and the header provisionally attached, you can reheat the pin to melt the solder and reposition the header if alignment needs to be adjusted.

* Finally, solder the remaining pins on the header. This will be the basic process for attaching all other headers to the board, so we will not reiterate the whole process each time.

![The pH carrier header attached to PCB](/assets/images/attached_header.jpg)

## Attach header for the keypad
Using the same method you used to attach the pH carrier board female header, solder on the 5-pin male header for the keypad. Make sure that these pins are placed on the opposite face of the PCB as the Arduino header pins.
![Keypad header](/assets/images/keypad_header.jpg)

## Potentiometer
Solder on the potentiometer. Make sure this component is soldered onto the same face of the PCB as the Arduino header pins.
![Poteniometer being soldered into the PCB](/assets/images/potentiometer.jpg)

## 3.5 mm PT100 jack
Solder the 3.5mm PT100 jack onto the same face of the PCB as the Arduino header pins.  This component has larger solder pins and will require more solder.
![3.5mm audio jack](/assets/images/audio_jack1.jpg)

![3.5 mm jack solder points](/assets/images/audio_jack_solder_points.jpg)

## Realtime clock female headers
Solder on a 5-position female header on the Real Time Clock location on the PCB on the same face as the Arduino header pins.
![Real Time Clock Header](/assets/images/RTC_header.jpg)

## LCD Header
Solder on a 16-position female header onto the LCD1 position on the opposite face of the PCB from the Arduino header pins.
![LCD Header](/assets/images/LCD_Header.jpg)

## Power screw terminals
Solder on the large screw terminals onto the PCB onto the face opposite the Arduino header pins in the location labeled "Power_Screws1". The openings on the side of the terminals (where the wires will be fed) should be facing toward the "AC Receptacle" location on the PCB.
![Power screw terminal 1](/assets/images/screw_terminal1.jpg)

![Power screw terminal 2](/assets/images/screw_terminal2.jpg)

## Jumper pins
Solder 5 3-pin male headers onto the positions labeled "LCD POT", "LCD RES", "LCD VDD", "RTC", and "PT100" inside the Arduino header pins, but on the opposite face of the PCB rom the header pins.
![Jumper pin positions](/assets/images/jumpers1.jpg)

Since these pins will be on the opposite face as the Arduino header pins, and therefore you will be soldering on the side with the long Arduino header terminals, you will need to use a rather steep angle with your soldering iron.
![Jumper pin soldering](/assets/images/jumpers2.jpg)

![Jumper pin soldered](/assets/images/jumpers3.jpg)

Once they are soldered on, place jumpers between the center pin and the "Arduino" pin on each header.
![Jumper positions](/assets/images/jumpers4.jpg)

## AC Power receptacle
Next, solder the AC receptacle onto the opposite face of the PCB from the Arduino header pins.  
![The AC Receptacle](/assets/images/AC_Receptacle.jpg)

I find the easiest way to do this is to hold the AC receptacle from underneath the PCB into it's through holes and then place a small chunk of solder near on of the terminals.
![The AC Receptacle being held to the board with a solder chunk next to a pin](/assets/images/AC_solder_chunk.jpg)

Then I can solder on that pin with that solder chunk.
![Soldering on AC receptacle first pin](/assets/images/AC_Soldering.jpg)

Then I can easily solder the remaining pins.

## Attach buck converters

Long wires on the bottom of the buck convert should be trimmed before soldiering.

Once pins are in place, they can be attached to the PCB.

Note the placement of the 9v and 5v volt buck converters. Must be placed in the correct location



## 2 Relay soldier pins and put on board

## Temperature break out board

* Break jumper
