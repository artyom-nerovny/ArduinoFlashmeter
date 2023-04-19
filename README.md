# ArduinoFlashmeter
Digital Arduino photographic flashmeter using BH1750 sensor and SSD1306 display.
Based on https://github.com/vpominchuk/lightmeter project.

Main components:
1. Arduino NANO v3 (ATmega328)
2. BH1750
3. SSD1306 display
4. Li-Po power cell
+ buttons, board, encoder etc.

Legacy functions list:
* Ambient light metering
* Flash light metering
* ND filter correction
* Aperture priority
* Shutter speed priority
* ISO range 8 - 4 000 000
* Aperture range 1.0 - 3251
* Shutter speed range 1/10000 - 133 sec
* ND Filter range ND2 - ND8192
* Displaying amount of light in Lux.
* Displaying exposure value, EV
* Recalculating exposure pair while one of the parameter changing
* Battery information
* Power 2xAAA LR03 batteries

TODO:
1. First of all, go from 2xAA batteries to 3,7v li-po cell. Add charge controller with Type-C USB.
2. Add parameter control with side wheel rotary encoder.
3. Change "METERING" button to side trigger-style smth.
4. Add common sync cable contact (if I find one: hot shoe mount) and update flash metering code.
5. Turn BH1750 to front. Update code for reflected light metering. (optional: use double back and front BH1750 sensors for both reflected and falling light measurements)
6. Add simple pit and/or lens for front sensor that cause smaller measure angle.
7. Add some sort of viewfinder.
8. Do some UI changes.
9. Develop all-in-one board with minimal ATmega328 chip necessary parts. So use ISP programmer.
10. Make sweet case :)