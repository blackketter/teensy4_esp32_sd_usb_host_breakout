A jumbo breakout board with ESP32, USB-A host and microSD connectors to mate with the [Teensy 4 Header Breakout Board](https://github.com/blackketter/teensy4_header_breakout).

It's designed to mount above or below the Teensy 4 and Header Breakout board on a relatively tall header.

Designed in KiCad.

Notes:

- In progress.
- [OSHPark order](https://oshpark.com/shared_projects/X9b5MPJw)
- Download bom/ibom.html and view it with web browser to see bill of materials and placement information.
- The last pin on the right side provides an optional enable pin for the power management chip on digital pin 27.  For always-on, cut left trace and short right two pads.  
- The last pin on the left side provides SD card detect on digital pin 29.  Needs INPUT_PULLUP.  Cut the jumper to free up pin 29.

![breakout render](render.png)
![breakout render_back](render_back.png)
![schematic](schematic.png)

Left Side Pinout:

1. 34/SD DAT1
2. 35/SD DAT0
3. GND
4. 36/SD CLK
5. 3.3V
6. 37/SD CMD
7. 38/SD DAT3
8. 39/SD DAT2
9. 29/Card Detect

Right Side Pinout:

1. VUSB
2. USB Host D-
3. USB Host D+
4. GND
5. GND
6. 27/EN

