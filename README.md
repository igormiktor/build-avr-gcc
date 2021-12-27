# build-avr-gcc
Scripts to build a complete avr-gcc toolchain

Currently it is a set of individual bash scripts to build:
* binutils targeting AVR (including patching size to include a special AVR output option)
* gcc targeting AVR
* avr-libc
* avrdude
* gdb targeting AVR


Your mileage may vary...

**Note:** All gcc versions after 7.5.0 generate bad code with a specific piece
of complex AVR code targeting the ATmega2560 that is important to me.  I
haven't invested the time to chase down the problem...
