# FirOS
## An OS for the Teensy 4.1 microcontroller.
#### Please note that this is still in development, and this document simply provides an outline of the os, and resources, such as installation guides, for when it is done.
### About
FirOS is not your typical operating system - in fact, you can only barely call it one. Here are the things that set it apart:

- It is written for a microcontroller, not a full-on computer. Typical operating systems are written for machines with a keyboard, mouse and internet access, however, this os is written for machine with none of those. It has basic IO, making it possible to add those things, but the OS itself does not make any attempt to drive them. Instead, it accepts commands and returns responses over a UART interface.
- It is written in MicroPython. Typical operating systems are written in assembly and C, but this os is written in MicroPython. However, MicroPython is considered more of a piece of firmware, rather than an operating system, meaning that this is could still be considered an OS - however, that is debatable, due to the fact that MicroPython acts like an operating system in some senses.
With this all in mind, I still consider this to be an operating system, however, I remain reluctant to go throwing the term around too much, because of the lack of similarities.

## Overview
FirOS is meant to be installed on a MicroSD card of suitable size, although the exact specifications cannot be determined yet. The uSD card also acts as the file system, much like with the Raspberry PI, so really, just go with whatever size you will be needing. However, be wary - I HAVE NOT DONE ANY TESTS TO DETERMINE IF THIS OS IS COMPATIBLE WITH MICRO-SD CARDS ABOVE 32GB, SO I HIGHLY RECOMMEND YOU BUY EITHER AT OR BELOW THAT NUMBER. \
\
FirOS comes with a small range of very obscure programming languages ported to MicroPython from GitHub, and also features implementations of sub-sets of others. There are also a few "adapted" languages available (versions of programming languages that have been given extra access to the machine, ect.) \
\
You can install a few drivers that I might release for this later, but at this stage, I consider this to be an in-development beta, so please don't expect much. The code is not even released yet for the actual os, so yeah, thats how fast development is going... :]. \

## System Requirements
This operating system requires the following to run:

- A Teensy 4.1 - This should be flashed with MicroPython, and have [LuBOOT](pigeon-nation.github.io/luboot) loaded into the onboard FLASH memory.
- A 32GB or less MicroSD Card

## Flash Requirments
- A computer capable of flashing to the Teensy 4.1, running the MicroPython mpremote tool, and writing to a MicroSD card. This means most Windows, Mac and Linux machines should work fine.
- A MicroUSB cable and USB Port.

## Installation Instructions
### Flashing your Teensy 4.1 with MicroPython
Step 1: Go to the MicroPython website and [download](https://micropython.org/download/TEENSY41/) the HEX file for the latest stable release of MicroPython (in bold) (at the time of writing, it is version 1.20.0. This may be different. Ignore the nightly builds).
Step 2: Go to the PJRC website and [download](https://www.pjrc.com/teensy/loader.html) the Teensy Loader *COMMAND LINE VERSION*. Follow the compile from source instructions. Make sure `make` works on your system.
Step 3: Download and install LuBOOT (unreleased). Follow the LuBOOT installation instructions.
ect. docs in progress.
