# Home Automation Using IoT - Adafruit & IFTT

This project mainly aims for making a 4 channel relay based IoT Control and getting various room sensor data like Gas, Temperatur, Humidity, Fire, etc. 

I made this project Inspired from Sachin Soni's Home Automation Projects, and have created a combined repository for all the necessary content.

### Basic Setup

The Libraries must be added to your local arduino installation before proceeding. Make sure you select NodeMCU and Enter Wifi Details as well as Adafruit Connection Details, before proceeding with upload.
In the Adafruit Dashboard add the necessary feeds/buttons necessary for the project. And the PCB gerber file is included, you can get them Printed or Use the Raw Schematics to make your own one.

### Components List

ESP8266 12e development board(NodeMCU) (http://amzn.to/2BKS7cv)
4 x 5V Relays (http://amzn.to/2ChddQC)
4 x 1n4007 Diode (http://amzn.to/2EM4IuD)
4 x BC547 transistors (http://amzn.to/2oiTbfV)
4 x 330ohm resistors (http://amzn.to/2ojg8zN)
16 channel analog multiplexer module (http://amzn.to/2mLwlfl)
PIR motion sensor (http://amzn.to/2EK1OX2)
MQ35  sensor
Sound Sensor (http://amzn.to/2HCYO0z)
Light Sensor (http://amzn.to/2CcBAPr)
DHT11 Temperature and Humidity sensor(http://amzn.to/2sPh3fO)
7805 Regulator IC (http://amzn.to/2CdUvcq)
9V Power Adapter (http://amzn.to/2CfffAL)
4 x 2 pin PCB mount screw terminal (http://amzn.to/2EM5Luz)

### Integration with Google Assistant

This project takes the help of two online platforms, IFTTT and Adafruit MQTT . IFTTT stands for If This Then That, its a great platform on which we can merge two services by making an applet. In this, we need to provide one condition and one action. The Action will be performed whenever the particular condition will be satisfied.
With the help of IFTTT, I’m merging Google Assistant and Adafruit MQTT. The applet which I made is something like,

> If Google assistant listens to turn on fan, then send data 1 to fan feed of Adafruit MQTT broker.

So this is one kind of applet which I made using IFTTT which combines my Google Assistant and Adafruit MQTT. Now how does Adafruit MQTT works? Basically, MQTT works on Broker Client Publish Subscribe method in which Clients are subscribed to one topic on the broker. Any data change in that topic will be reflected to all the devices connected to that same topic in that broker.
MQTT broker can be a local broker that works in the range of a wifi router, or it can be a cloud based broker that works from anywhere in this world.

#### For Further Learning 
Get Started with MQTT Broker & Create a Local Broker using any youtube link.

For queries,do connect with me via [My Website](https://dipanroy.com)
