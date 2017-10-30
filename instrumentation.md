# Instrumentation

To start taking data you need the brain of your circuit! We suggest using a [Raspberry Pi 3](https://www.amazon.com/Raspberry-Model-1-2GHz-64-bit-quad-core/dp/B01CD5VC92). This can connect directly to AWS IoT which makes it a lot easier then using an Arduino which we used in our first prototype. 

This was an interesting one for us. All of us previously had expirience with Ardiuno but had never really used Raspberry Pi before. Here are a few problems we ran into.
1. When setting up your Raspberry Pi you need an HDMI Cord to a monitor, a USB Keyboard and a USB Mouse. You need to configure the Pi so it can be accessed remotely on a laptop (or phone) using an SSH code. This is easier if you configure the IP address to be constant. 
2. You may need to purchase a router. At UBC Wi-Fi requires a secondary login. This is hard to get past on a Raspberry Pi for some reason. We purchased a router and set up our own Wi-Fi. This was also beneficial as there is not as much traffic on the network. 

The most important basic measurement in brewing is temperature. **Temperature is essential to the flavor of the beer**. We suggest purchasing the DS18B20 Waterproof Temperature probe. On the brewing page we recommend purchasing a thermowell. This is so you can place your temperature sensor inside the fermenter without the sensor being in contact with the fluid. While the temperature sensors are waterproof this saves you the step of sanitizing them and the temperature profile in the fermenter is actually most accurate in that location as the fluid conducts the temperature throughout the thermowell. We set up an ambient temperature sensor as well to measure the ambient temperature which gives us an idea of how the temperature in the fermenter might flucuate as the temperature approaches equilibrium. The sensors we purchased have an uncertainty of 0.5 degrees Celsius which is a little too high for my liking. I recommend purchasing something more accurate. 

