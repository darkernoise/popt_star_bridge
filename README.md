# popt_star_bridge
PopT Star Sensor Bridge is an open-source project, designed around the Raspberry PI, that makes setting up home automation sensors quick and easy.  Just download a full pre-built image file, write it to an SD card, connect up a few sensors to the Raspberry PI, edit a text configuration file to define the sensors, and the sensor is now available wirelessly within your home.

Types of sensors that interface with PopT Star Sensor Bridge:

Standard Alarm Sensors: 
* Standard binary alarm sensors, such as magnetic reed sensors, motion detectors, glass break sensors, water leak sensors, basically any alarm sensor with a “normally open” or “normally closed” loop.

I2C/TWI: 
* Generic I2C Sensors:  Any I2C sensors that return a simple packet of data bytes can be configured.
* Complex I2C sensors such as the BPM280/BME280 (temperature, humidity, and atmospheric pressure) can direct connect to a Raspberry over the I2C connectors.  More complex I2C sensors will be added in the future.

Serial: 
* Serial sensors, such as the Plantower PMS7003 High-Precision Laser Dust Sensor can connect direct to a Raspberry PI over the serial connectors.  More serial sensors will be added in the future.

Analog and Arduino:  
* The PopT Analog to I2C Arduino sketch can be used to convert analog sensors to the I2C bus for connection to the Raspberry PI/PopT Star Sensor Bridge.  For example, connect up:
  * DHT22/AM2303 Temperature and Humidity Sensor
  * MQ-2 Smoke, Gas, and Butane Sensor
  * MQ-4 Gas Sensor
  * MQ-7 Carbon Monoxide Sensor
  * Sharp GP2Y1010AU0F Dust Sensor
