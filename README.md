SolarPower
==========

Using an Arduino with an Adafruit INA219 breakout board and a TIP120 transistor to monitor and control solar systems.

Voltage and current are logged to an SPI flash chip every 10 seconds.
A button is used in conjunction with a TIP120 transitor to turn on and off high-voltage devices. A low-voltage disconnect value can also be set to protect the battery from over-discharge.


Here's a Fritzing image of the circuit. The ? PCB is an INA219 breakout for monitoring the power consumption of the pump.

![The circuit](http://i.imgur.com/zYkL1aL.png)

Components
=================

* Rectifier Diode 1N4001
* 12V aquarium Pump (Motor on diagram)
* Arduino
* Male + Female Power plugs for pump. Pass-through ports for power. 
* TIP120	NPN-Power transistor to switch the pump on and off
* 4k Ω Resistor
* $2 RTC Module DS1302 from eBay
* INA219 for current monitoring.
* 

I used a Moteino from lowpowerlab.com to create this project! 

Requires the following arduino libraries:

Adafruit_INA219

SPIFlash

SPI

This sketch is based on the Adafruit_INA219 and SPIFlash example sketches.

