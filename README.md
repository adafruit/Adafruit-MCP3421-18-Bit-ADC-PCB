## Adafruit MCP3421 18-Bit ADC - STEMMA QT / Qwiic PCB

<a href="http://www.adafruit.com/products/5870"><img src="assets/5870.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit MCP3421 18-Bit ADC - STEMMA QT / Qwiic. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5870

### Description

The Adafruit MCP3421 18-Bit ADC is a simple, inexpensive, and easy to use 18-bit, 240 SPS, single-channel ADC with an I2C interface that can run up to 3.4MHz clock rate. A perfect component whenever you need an ADC that has differential inputs, adjustable gain, and a built in precision/low-drift reference voltage.

One of the trade-offs with getting 18-bit precision is that the ADC is not going to be very fast: you can configure the chip to do a faster 12-bit conversion at 240 SPS, but at 18-bits it slows down to 3.5 SPS.
That's because the way a sigma-delta ADC works, it 'guesses' the analog voltage and uses a comparator to determine whether the input is higher or lower. Each 'guess' takes an extra step, and thus
halves the throughput, so 12-bit is 240 SPS, and 14-bit is 1/4 (2-bit) slower, 60 SPS. Ditto 16-bit is 1/4 slower, 15 SPS, and finally 18-bit is 3.75 SPS.

The MCP3421 is already set up for differential inputs, which means that you can read positive or negative differences between the two inputs, as long as both signals are between 0 and 2.048V. This means its not going to be great for reading stuff like potentiometers, where you have a single-end reading referenced to ground, and you want to read the full range from 0 to Vcc. It is great, however, for reading sensors like strain gauges, pressure sensors, or thermocouples.

We have a ready to go Arduino library that makes usage simple: select the sample rate / precision you want and one-shot or continuous mode. Then read values over I2C! This sensor has a fixed address, so you may want to use a multiplexor if you want to connect multiple MCP3421's on a single I2C bus.

To get you going fast, we spun up a custom-made PCB in the STEMMA QT form factor, making it easy to interface with. The STEMMA QT connectors on either side are compatible with the SparkFun Qwiic I2C connectors. This allows you to make solderless connections between your development board and the MCP or to chain it with a wide range of other sensors and accessories using a compatible cable.

QT Cable is not included, but we have a variety in the shop.

Comes with a bit of 0.1" standard header in case you want to use it with a breadboard or perfboard. Four mounting holes for easy attachment.

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
