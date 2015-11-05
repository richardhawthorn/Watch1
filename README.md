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