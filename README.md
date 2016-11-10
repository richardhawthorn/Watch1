### Description

An Arduino multimeter watch

### Multimeter functions

- Displays voltage between 0 and 30v
- Displays current upto 500mA
- Zener clamp and 500mA PTC to protect Arduino

### Features

- ATMEGA328P with Arduino boot-loader
- 3.3V operation with CR2032 battery
- 32.768kHz crystal
- Mini 7 segment display
- 2x side buttons for menu operation
- FTDI programming port
- Low power operation

### Bootloader

You will need to set various fuses when you upload the bootloader, thse can be done with this command

avrdude -b 19200 -c usbtiny -p m328p -v -e -U lfuse:w:0xe2:m -U hfuse:w:0xda:m -U efuse:w:0x07:m

### License

This work is licensed under a Creative Commons Attribution-ShareAlike 4.0 International License.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />
Designed by <a xmlns:cc="http://creativecommons.org/ns#" href="http://www.richardhawthorn.com" property="cc:attributionName" rel="cc:attributionURL" target="_blank">Richard Hawthorn</a><br />
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/" target="_blank">View License</a>
