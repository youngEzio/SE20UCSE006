# SE20UCSE006
AI in Industry

**Contributors<br/>**
Rounak Das SE20UCSE149<br/>
Abhinav Chaudhry SE20UCSE006<br/>
Keshav Garg SE20UCSE065


<b>
Sensor used: Sound Sensor Module / Condenser Mic Sound Sensor<br/>
Actuator used: Buzzer
</b>

First, Raspberry pi 4 was configured. We used a 64GB SD card where we flashed RaspiOS using Rasberrypi Imager.
There we configured our hostname, Wi-Fi (hotspot) and enabled SSH access.

After that, we connected Raspberrypi to a monitor using MicroUSB-HDMI and HDMI cable. (This is optional)

We ssh-ed into raspi using our laptop after that and pasted the code `sound.py`

We used a sensor called Sound Sensor Module / Condenser Mic Sound Sensor. 
From there, we took digital input into the Raspberry-pi using GPIO pin 17.

After that we set up an event callback (similar to interrupt in arduino) whenever our pin data goes HIGH or LOW.

Whenever a sound is detected (signal from GPIO pin 17), we play a buzzer for 2 seconds. 

The GPIO pin 23 is our ouput pin connected to the signal pin of the buzzer.

In a breadboard, VCC (5V) and GNDs are all connected in a rail.


