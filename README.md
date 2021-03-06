# SERVER communications with Android Things on Raspberry Pi 3 B
## Features
A simple Android application running on Raspberry Pi 3 with those functions:

* Write blocks of data to an RFID card including
➢ Name, DOB, Student ID
➢ Authenticate if possible

* Continuously read an UID and the written data from an RFID card and display this information on a screen.

* Turn the green LED of an RGB LED on when the card of one of your group members is presented.

* Flashing the red LED of an RGB LED 5 times in 2 seconds when the other cards are presented.

* By default, the blue LED of an RGB LED is turned on, and only one LED is turned on at a time.

Additionally, with every successful reading, the UID of the tag will be sent to a remote server.
## Connection
| Raspberry PI 3 | Peripherals     | 
| -------------- | ---------------:| 
| BCM2           | LED Red         | 
| BCM3           | LED Green       | 
| BCM4           | LED Blue        | 
| BCM8           | SDA - RC522     | 
| BCM11          | SCK - RC522     | 
| BCM10          | MOSI - RC522    |
| BCM9           | MISO - RC522    |
| BCM25          | RST - RC522     | 
* Please note that based on your LED, the LED's common pin might be connected to Vcc or GND.
* Also keep in mind that Button's pins must be wired so that it is active low (using a resistor might help).
* The MFRC522 module works with 3.3V.
## Usage
* This application is the combination with the Lab 03. However, now UI is added.
* Click on Write button to write to the tag with predefined information.
* Click on Read button to read information from the tag and display it onto the screen.
* During reading and writing serivces, click Stop button to stop those.
* Upon reading successfully, the tag's UID will be sent to the server at: http://demo1.chipfc.com/SensorValue/List/7
## Members
1. Minh-Duc Hoang-Nguyen, 1610755
2. Thanh-Linh Thai-Thi, 1611830
3. Thinh Le-Duc, 1613346
4. Thinh Le-Minh, 1513249
## Info
* Bach Khoa University, Faculty of Computer Science and Enginnering
* Computer Engineering Department
* IoT Application Development - Fall 2018
* LAB 04
### Instructors
1. Le Trong Nhan, Ph.D
2. Nguyen Tran Huu Nguyen, Ph.D

