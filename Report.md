# RFID-Door-Lock
RFID Door Lock with Bluetooth using Arduino 
-
The purpose of this project is to design a
smart locking system using Arduino,
allowing the electric solenoid lock to be
opened in two different ways: by using an
RFID card or through Bluetooth
communication using the HC-05 module.
The system provides a simple and secure
method for access control

what you need to make this project
-
1-Arduino
2-RFID sensor
3-Relay Module
4-Bluetooth (hc-05)
5-breadboard
6- 2 resistor(1k ohm and 2k ohm)
7- 12v battery or power supplay
8-electric solenoid 12v

How this project works
-
first we identify the card by using code to get the id of the card we will use
then we will take the id and identify to the arduino 
so if we pass the card to the rfid sensor the sensor will read the id and transfer it to the arduino
after that the arduino will cheak if the id we got from the sensor is the same as the id we write it earlier
if it the same it will send a signal to pin 7 
the pin 7 is connected to the relay (signal-pin)
then the NO (Normally Open) in the relay will connect to the COM (Common)
and make the solenoid run for 2s

for the bluetooth 
-
we have 2 resistor shown in image.png
the purpose of the 2 resistor is to make voltage divider
so in RXD pin we need 3.3V from the arduino
and pin 3 is given 5V
so if we 5*(1000/2000+1000)=3.3V
after that if we connected the the bluetooth via the phone and send a code 
the code will be sent to the arduino and compare it to the code that we write it in the code earlier
if it's ,the pin 7 will run for 2s after that will turn off 

