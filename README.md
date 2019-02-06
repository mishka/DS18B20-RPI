# About
I was using this to monitor my aquarium's temperature.

# Requirements
- Python3
- Tweepy  
- RPI
- DS18B20
- 4.7K Ohm or 10K Ohm resistor

# Setup before running
- Connect the sensor to the rpi.  
![alt tag](https://cdn1.imggmi.com/uploads/2019/2/7/0b6cd6047c213e7c06d3baf5928de3da-full.png "circuit")
- Add ```dtoverlay=w1–gpio``` to ```/boot/config.txt```.
- Reboot.
- Open the terminal then type ```modprobe w1–gpio``` and ```modprobe w1-therm```.
- Go to the folder ```/sys/bus/w1/devices``` and look for a folder starting with ```28-XXXXXXXXXXXX```.

If it's there, it means that you connected the cables successfully.  
If not, reconnect the wires then try again.
