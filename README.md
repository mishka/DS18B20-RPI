# requirements
- python3
- tweepy  
- rpi
- ds18b20
- 4.7K ohm or 10K ohm resistor

# setup before running
- Connect the sensor to the rpi.  
![alt tag](https://cdn1.imggmi.com/uploads/2019/2/7/0b6cd6047c213e7c06d3baf5928de3da-full.png "circuit")
- Add ```dtoverlay=w1–gpio``` to ```/boot/config.txt```.
- Reboot.
- Open the terminal then type ```modprobe w1–gpio``` and ```modprobe w1-therm```.
- Go to the folder ```/sys/bus/w1/devices``` and look for a folder starting with ```28-XXXXXXXXXXXX```.

If it's there, it means that you connected the cables successfully.  
Reconnect the wires then try again if you can't see it.
