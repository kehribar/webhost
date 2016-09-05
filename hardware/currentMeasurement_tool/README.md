Presicion current measurement tool with low burden voltage 
================

This is my attempt to create a battery powered and isolated digital presicion current measurement tool with low burden voltage. Dave L. Jone's uCurrent [http://www.eevblog.com/projects/ucurrent/](http://www.eevblog.com/projects/ucurrent/) board was my inspiration to create this design. 

What I've learned from the uCurrent design is that one way to have a low dropout voltage while maintaining to have a high accuracy when making current measurement is to amplifiy the shunt voltage with a known gain. I've used a application spesific instrumentation amplifier from Analog Devices named AD8293 [http://www.analog.com/static/imported-files/data_sheets/AD8293G80_160.pdf](http://www.analog.com/static/imported-files/data_sheets/AD8293G80_160.pdf). Gain of this amplifier is fixed, which eliminates the need for a high precision resistors.

I've used an 18bit ADC from Microchip named MCP3422. This ADC has its own built-in voltage reference which eliminates the need for an external voltage reference. Lastly, I've used an I2C isolation chip from TI to isolate the battery operated circuit via the I2C host side.

I've ordered parts for this board but haven't populated and tested yet ...

### Schematic

![image](current_measure_sch.png)

### Layout

![image](current_measure_brd.png)

### Build

![image](current_measure_build.jpg)

