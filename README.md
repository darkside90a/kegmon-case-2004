# kegmon-case-2004
A KegMon case for 2x 2004 LED displays

You find a complete description of mp-se's great KegMon project here:

https://github.com/mp-se/kegmon

It all started when v0.7 came out with support for 20x4 LED displays.
I wanted to build a new case!

And I wanted to have a case with the displays beside each other to match the
taps rather than above each other.
Instead of making one, I found an IP65 ABS plastic case 250x80x70mm on Ebay suitable.

I made a base plate of 3mm acrylic to fit inside the box with hole patterns for
2x displays + one 60x80mm experiment PCB:

![bunnplate-20230910](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/7dbfbebc-1f29-44a1-bfec-727772b383fc)
Sorry, the dxf (bunnplate-20230910.dxf) is a bit dodgy.



I made holes for the displays in the lid by using a 1:1 printout as a template.
The holes were filled by gluing CNC'ed acrylic "windows" (display-tc2004.stl) in place

![P1010722](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/089cc791-bc73-4fe9-a829-49e5a33cf142)


I have re-designed mp-se's PCB a little bit to match hole patterns of the 2004 displays.
Width is made the same as the 2004 displays.
Mechanical holes for the HX711's were removed, and the 5V terminal was moved to not
interfere with the USB-C connector of the ESP32-S2.
The changes gave me the opportunity to re-route some traces and make them beefy enough 
to mill the PCB on my CNC3018 (kegmon_hx711-Bot-2.0.gbr kegmon_hx711-2.0.drl).

![P1010735](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/d6f12b4b-7196-4230-8348-706fe78fba12)


First "layer" with M3 nylon standoffs and PCB's:

![P1010736](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/fff6e061-0267-441e-85f1-7e0e2369c256)
![P1010737](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/86c49286-be7c-426d-83df-d547086fd680)


Most of the Dupont cables and nylon standoffs are in place. USB-A on the experiment PCB
is power input. It is connected to rows of pins to distribute 5V around.
The small PCB on the experiment board is a 4x bidirectional logic level converter.
I run the displays on 5V, and needed to lower SDA/SCL from them to 3.3V

![P1010739](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/18f84539-db2c-4951-b188-97b043240d6d)


All in place, ready for flashing and 1st test before disassembly and reassembly in the case.
There is lots of space. Enough to fit a small 230/5V PSU in the experiment PCB area.

![P1010740](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/054aafd3-1c45-487b-878b-7e4fd06f2cfd)


Final test after assembly. I just need to copy settings from the "old" case before 
connecting it to the scales in the keezer. 

The design is symmetrical. If connectors are wanted on the "front" side instead of rear, just rotate/swap displays.  

![DSC_1779](https://github.com/darkside90a/kegmon-case-2004/assets/52971840/29cefacf-e694-41a8-8ffe-90388a365882)

