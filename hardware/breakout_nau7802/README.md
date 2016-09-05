NAU7802 - 24bit ADC breakout board
================

nau7802 is a great and very affordable 24 bit ADC with reasonable slow sampling rate. The chip itself can be bought at 1.8$ in single quantity from Digikey: [http://www.digikey.com/product-detail/en/NAU7802SGI/NAU7802SGI-ND/2769782](http://www.digikey.com/product-detail/en/NAU7802SGI/NAU7802SGI-ND/2769782) 

I've used and precision 3V voltage reference to drive the ADC's VRef pin. In this configuration, chip can read +/- 1.5V between its differential inputs. Chip outputs the measured value in 2's complement form. Also, even though the chip supports maximum 320 SPS (samples per second), it works best at 10 SPS. Lasty, I've connected the board's VCC into the second channel of the ADC via a voltage divider to measure the VCC voltage. 

I've used this board to precisely measure a voltage which has slow changing rate. I also written a library to use this chip but haven't published it yet.

### Schematic

![image](nau7802_sch.png)

### Layout

![image](nau7802_brd.png)

### Build

![image](nau7802_build.jpg)

