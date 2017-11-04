# Instrumentation

To start taking data you need the brain of your circuit! We suggest using a [Raspberry Pi 3](https://www.amazon.com/Raspberry-Model-1-2GHz-64-bit-quad-core/dp/B01CD5VC92). This can connect directly to AWS IoT which makes it a lot easier then using an Arduino which we used in our first prototype. 

This was an interesting one for us. All of us previously had expirience with Ardiuno but had never really used Raspberry Pi before. Here are a few problems we ran into.
1. When setting up your Raspberry Pi you need an HDMI Cord to a monitor, a USB Keyboard and a USB Mouse. You need to configure the Pi so it can be accessed remotely on a laptop (or phone) using an SSH code. This is easier if you configure the IP address to be constant. 
2. You may need to purchase a router. At UBC Wi-Fi requires a secondary login. This is hard to get past on a Raspberry Pi for some reason. We purchased a router and set up our own Wi-Fi. This was also beneficial as there is not as much traffic on the network. 

The most important basic measurement in brewing is temperature. **Temperature is essential to the flavor of the beer**. We suggest purchasing the DS18B20 Waterproof Temperature probe. On the brewing page we recommend purchasing a thermowell. This is so you can place your temperature sensor inside the fermenter without the sensor being in contact with the fluid. While the temperature sensors are waterproof this saves you the step of sanitizing them and the temperature profile in the fermenter is actually most accurate in that location as the fluid conducts the temperature throughout the thermowell. We set up an ambient temperature sensor as well to measure the ambient temperature which gives us an idea of how the temperature in the fermenter might flucuate as the temperature approaches equilibrium. The sensors we purchased have an uncertainty of 0.5 degrees Celsius which is a little too high for my liking. I recommend purchasing something more accurate. 

## *TASKS COMPLETED TO DATE:*

1. Obtain Raspberry Pi and sensors
2. Review datasheets for raspberry pi and sensors 
3. Configure the raspberry pi 
4. Preliminary hardware setup 
	-Gather materials (breadboard, resistors, wires)
  	-Connect the first thermometer to the raspberry pi according to the specifications identified in the sensor and raspberry pi datasheets
5. Data acquisition and testing (see notes under software team’s recap)
	- Obtain temperature reading from the temperature sensor
	- Software team set the sampling time and refined script for monitoring
6. Add a second temperature sensor
7. Software team reviewed and updated script to obtain reading from both temperature sensors
8. Addition of pH sensor to circuit (note a couple connections have been left open to avoid unnecessarily powering the sensor while not in use, however all pin and connection locations have been identified)
9. Implement a switch button to control data acquisition (in progress)

## NEXT STEPS:
Write a script to execute data monitoring script upon start-up

Set up the button to control the power of the raspberry pi (effectively acting as a on/off switch).This will require minor hardware modifications and an additional script.

Write a script for pH data acquisition 

Determine logistics of how to obtain pH measurements (sensor placement)

Integrate weight sensor into the sensor system

Review specification sheet to determine electrical and physical requirements

Identify a suitable mounting location

Determine which raspberry pi pins would be most suitable and make connections

Write a script for weight sensor data acquisition

## RESOURCES

### Temperature Sensor
Datasheet: https://datasheets.maximintegrated.com/en/ds/DS18B20.pdf

General Info: https://www.maximintegrated.com/en/products/analog/sensors-and-sensor-interface/DS18B20.html/tb_tab0

### Raspberry Pi
Interactive pin layout: https://pinout.xyz/

Hardware guide: https://www.raspberrypi.org/learning/hardware-guide/

Initial Setup: https://www.raspberrypi.org/learning/hardware-guide/quickstart/

How To Be a Maker- A guide to Arduino and Raspberry Pi 2 (info and link to free download here: https://diyhacking.com/arduino-projects-raspberry-pi-projects/ )

Access to GPIO with Python on Your Raspberry Pi 3: https://www.arrow.com/en/research-and-events/articles/raspberry-pi-gpio 

### Temp Sensor Tutorials using Pi:
A good sample tutorial showing two temp sensors integrated with raspberry pi: http://projects.privateeyepi.com/home/temperature-sensor-project-using-ds18b20

https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/temperature/ 
