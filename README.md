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

**Note:** Also, turns out that the last version of gcc officially supported by the AVR chip vendors
(Atmel/Microchip) is v7.3.0.  I've used v7.5.0 extensively without any problems.  However, if you 
want to be safe, you can edit the gcc version in `avr-file-names` to 7.3.0. 
