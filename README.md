# requirements
- python3
- tweepy  
- rpi
- ds18b20
- 4.7K ohm or 10K ohm resistor

# setup before running
- Connect the sensor to the rpi.
![alt tag](https://pasteboard.co/HZXPyLa.png "circuit")
- Add ```dtoverlay=w1–gpio``` to ```/boot/config.txt```.
- Reboot.
- Open the terminal then type ```modprobe w1–gpio``` and ```modprobe w1-therm```.
- Go to the folder ```/sys/bus/w1/devices``` and look for a folder starting with ```28-XXXXXXXXXXXX```.
- If it's there, it means that you connected the cables successfully.
- Reconnect the wires and try again if you can't see it.
