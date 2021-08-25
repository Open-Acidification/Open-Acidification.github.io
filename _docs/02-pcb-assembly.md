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

3. Next, remove solder from the through-holes by placing the aperture of the solder sucker directly over a through hole, while simultaneously heating the solder in the through hole with the soldering iron.
  When the solder liquefies, fire the solder sucker to remove the solder from the hole.
  You may need to repeat this step multiple times per through-hole to completely clear the hole of solder.
  Be careful not to leave the soldering iron on the through-hole too long and cause the pad to separate form the PCB.  

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

![Finished buck converter](/assets/images/finished_buck_converter.jpg)

## Soldering Arduino Header Pins

![Arduino, 2.5 mm header pins and custom pcb]()

* Arduino Mega
* 1x 2.54 mm 4 header pins
* 1x 2.54 mm 6 header pins
* 1x 2.54 mm 2x18 header pins
* Custom PCB

![Arduino Pins Layed Out](/assets/images/Arduino_Header_Layout.jpg)

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
Using the same method you used to attach the pH carrier board female header, solder on the 8-pin male header for the keypad. Make sure that these pins are placed on the opposite face of the PCB as the Arduino header pins.
![Keypad header](/assets/images/keypad_header.jpg)

## Potentiometer
Solder on the potentiometer. Make sure this component is soldered onto the same face of the PCB as the Arduino header pins.
![Potentiometer being soldered into the PCB](/assets/images/potentiometer.jpg)

## 3.5 mm PT100 jack
Solder the 3.5mm PT100 jack onto the same face of the PCB as the Arduino header pins.  This component has larger solder pins and will require more solder.
![3.5mm audio jack](/assets/images/audio_jack1.jpg)

![3.5 mm jack solder points](/assets/images/audio_jack_solder_points.jpg)

## Realtime clock female headers
Solder on a 5-position female header on the Real Time Clock location on the PCB on the same face as the Arduino header pins.
![Real Time Clock Header](/assets/images/RTC_header.jpg)

Solder on a 5-position female header on the Real Time Clock location on the PCB on the same face as the Arduino header pins.

![Real Time Clock Header](/assets/images/RTC_header.jpg)

## LCD Header
Solder on a 16-position female header onto the LCD1 position on the opposite face of the PCB from the Arduino header pins.
![LCD Header](/assets/images/LCD_Header.jpg)

Solder on a 16-position female header onto the LCD1 position on the opposite face of the PCB from the Arduino header pins.

![LCD Header](/assets/images/LCD_Header.jpg)

## Power screw terminals
Solder on the large screw terminals onto the PCB onto the face opposite the Arduino header pins in the location labeled "Power_Screws1". The openings on the side of the terminals (where the wires will be fed) should be facing toward the "AC Receptacle" location on the PCB.
![Power screw terminal 1](/assets/images/screw_terminal1.jpg)

![Power screw terminal 2](/assets/images/screw_terminal2.jpg)

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
Now place the buck converters onto the PCB on the same face as the Arduino header pins.  The through holes for these converters are slightly closer together on the PCB than on the converters.  This is intentional so that you can place them and have tension keep them in place while you test the units before soldering them on.  Make sure that you place the correct buck converter in the correct place on the PCB. The positions are marked on the PCB. The 5V buck converter should have a 1000 &mu;F capacitor on the output end, the 9V should have a 470 &mu;F capacitor in the same position.
![Placing buck converters on PCB](/assets/images/buck_placement.jpg)

### Testing buck converters before soldering
Before soldering the buck converters to the PCB you should test the outputs to make sure 1) that you placed the buck converters in the correct positions and 2) that the converters are not defective. To do this we need to plug the board into an outlet, which must be done very carefully to prevent giving yourself a very dangerous shock.  To do this safely, first secure the PCB so that it remains in place while plugged in. I suggest using a PCB holder for this.  Then, plug the power cable into the PCB.  Only then plug the power cable into a wall outlet. Once the PCB is plugged into the wall, DO NOT TOUCH IT except with the multimeter.  If you need to reposition the board, unplug it from the wall before doing so.  

Once you have the PCB secured and plugged in, use a multimeter to check the voltage output on both the 5V and the 9V buck converters. This is most easily done on the pins protruding through the PCB on the opposite face of the buck converters.
![Checking voltage of buck converters](/assets/images/check_voltage_buck.jpg)

It is also useful to check the 7V power output from the screw terminal block for the arduino. You can do this by checking voltage between the screws labeled "To Arduino VIN/9V" and "AC-E".
![Checking voltage of arduino power](/assets/images/check_arduino_power.jpg)

### Soldering buck converters in place
Once you have check the voltage outputs of the buck converters, confirming correct placement and that they are in working order, you can solder down those two devices.  Before you do this, however, UNPLUG THE PCB BEFORE MOVING OR ATTEMPTING TO SOLDER the buck converters.
After you have solders all 4 pins on each buck converter, you can trim the pins on the opposite face from the buck converter with a wire cutter.

## PT100 temperature probe break out board
Next we will attach the headers and configure the MAX31865 PT100 temperature probe break out board.  You will need the 8-pin male header that came with the breakout board, a 8-pin female header, three 1-pin female headers, and clip off 3 1-pin headers from the spare 16-pin header as you did with the buck converters.  You will not need the two screw terminals that come with the pt100 breakout board.
![Parts needed to attach the pt100 temperature probe](/assets/images/pt100_parts.jpg)

To attach the board to the PCB, first place the 8-pin male header into the 8-pin female header.
![8-pin header attachment](/assets/images/pt100_8pin_apart.jpg)
![8-pin header attached](/assets/images/pt100_8pin_together.jpg)

Next, place the 1-pin male headers into the 1-pin female headers.
![1-pin header attachment](/assets/images/pt100_1pin.jpg)

Place each of these mated male/female headers into the PCB on the position marked "PT100 Amp", with the pins for the female headers placed into the PCB.  There are 3 single pin headers, but 4 positions to place them.  Place them into the three positions closest to the edge of the the PCB.
![PT100 header placement on the PCB](/assets/images/pt100_pins_placed.jpg)

Then, place the pt100 breakout board on the male side of the header pins and solder into place.
![PT100 breakout board soldered into place](/assets/images/pt100_soldered.jpg)

Following soldering the pt100 breakout board, you can also solder the female header pins on the PCB.  

### Configuration of the PT100 breakout board
On the PT100 breakout board solder together the pads that are labeled "2/3Wire"
![2/3 wire jumpers](/assets/images/pt100_jumper1.jpg)

Next, use a sharp instrument (I use the pointed tip of my wire cutters) to cut the jumper between the "2" and "4" pad on the "2 4   3" jumper.
![243 wire jumpers](/assets/images/pt100_jumper2.jpg)

Finally, on that same jumper set, solder together the "4" and "3" pads.
![243 wire jumpers soldered](/assets/images/pt100_jumper3.jpg)

## Attach real time clock breakout board
Solder the header pins that came with the PCF8523 Real Time Clock breakout board. I generally do this by placing the header pins on a breadboard, then placing the breakout board on top of that to solder the pins on.
![Real Time Clock attached](/assets/images/RTC_breadboard.jpg)

Then place on the female header on the PCB.  Finally, put a CR1220 coin battery into the breakout board.


## Attach the Atlas Scientific EZO pH breakout board
Remove the electrically isolated EZO carrier board from the packaging, and attach the header as you did with the RTC breakout board.
![EZO pH packaging](/assets/images/EZO_pH_packaging.jpg)
![EZO pH carrier board placed on breadboard for soldering](/assets/images/EZO_pH_carrier.jpg)

Next, place the red EZO pH stamp on the carrier board so that the "PH EZO" lettering is closest to the large white plastic part of the carrier board and the BNC plug.  
![EZO pH stamp placed on carrier board](/assets/images/EZO_pH_stamp.jpg)

Finally, place the entire assembly on the "pH carrier board" position on the PCB by inserting the male header on the carrier board into the female header on the PCB.

## 2-relay module attachment
First, solder the 3-pin and 4-pin female headers onto the PCB on the side that is opposite the Arduino header pins. To make this easier, you may temporarily remove the real time clock, PT100 and EZO pH breakout boards from the PCB by unplugging them from the PCB and setting them aside.
![Soldering the 2-relay module female headers](/assets/images/relay_module_soldering.jpg)
![2-relay module headers](/assets/images/relay_module_headers.jpg)


Next, place the 2-relay module onto the PCB by plugging it into the female headers.
![2-relay module plugged into the PCB](/assets/images/relay_module_attached.jpg)

### Attaching high voltage wires to relay
Cut two pieces of stranded 14 gauge (AWG) wire to a length of approximately 3.5 cm.  
![high voltage sires to relay](/assets/images/wires_cut.jpg)

Strip the insulation of the last 5mm of each end.
![The relay wires stripped](/assets/images/wires_stripped.jpg)

Tin the ends of the wire where it is not covered by insulation.  This involves heating the bare wire with the soldering iron, and melting solder into the wire, allowing the strands to "wick" up the solder.
![Tinning the wire](/assets/images/wires_tinned.jpg)

Next, bend the wires approximately in the middle.
![The wires bended to fit the relay.](/assets/images/wires_bent.jpg)

Next, place on end of the wire in the middle terminal of each of the two 3-position terminal screw blocks on the relay module and place the other sides in the hole in the PCB labeled "Screw1" and "Screw2". Tighten the screws to secure the wires into place.
![attaching to breadboard](/assets/images/wires_placement.jpg)

Finally, solder the ends of the wires in the PCB to the holes.
![Soldered high voltage relay](/assets/images/wires_soldered.jpg)

Now, you are finished assembling the custom PCB.
