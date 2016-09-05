Intelligent electromagnet driver
================

During my senior year at the college, me and my teammates were working on a Human-Computer Interaction technology called [MagiTact](https://www.google.com/search?btnG=1&pws=0&q=Magitact) for our senior project. In this technology, a permanent magnet is used to manipulate the electromagnetic field arround a mobile device which then interfaces with the internal compass(magnetometer) of the device. By analysing this additional magnetic field, user interaction can be created between the user and the mobile device.

In our study, we created an electromagnet module which can modulates its output power in a spesific frequency. Our aim was to have a multi user interaction with a single magnetometer by demodulating the effects of different magnets in different frequencies at the host side.

This board has an opamp+transistor based constant current source to drive the electromagnet coil. Also there is a quad-mosfet based H-bridge circuit to be able to change the direction of the current flowing in the electromagnet. Sine wave is generated via an I2C based 12bit DAC. The output frequency of this bord can be changed over USB via CDC based serial interface. PIC18F13K50 microcontroller is used as the main controller. There is also a charging circuitry for LiPo batteries when the device is connected to the USB.

Routing for this circuit is all done by myself. After routing, this board is manufactured via a LPKF milling machine available at my university then silkscreen is applied to the board manually with additional LPKF tools. 

### Schematic

![image](modulator_sch.png)

### Layout

![image](modulator_brd.png)

### Build

![image](modulator_build.jpg)

