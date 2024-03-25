# Technical specification - Team 6 

# Coris Sport-Shield Project

This document will specify all the technical aspects of the project. 

## Technical Specification Approval

|**Name**               |**Role**           |**Signature**  |**Date**  |
|-----------------------|-------------------|---------------|----------|
| Evan UHRING           | Project Manager   |               |          |
| Jason GROSSO          | Program Manager   |               |          |
| Ian Laurent           | Tech Lead         |               |          |
| David CUAHONTE CUEVAS | Technical Writer  |               |          |
| Gaël MALVAR           | Software Engineer |               |          |
| Guillaume DERAMCHI    | Quality Assurance |               |          |

## Table of Content

## Introduction

This project was given to us on March 11th 2024 as a school project with the task to obptimise the code to be able to extend the battery life and reduce as much as possibke the battery consuption. 
As for the device the device consists of a anti-theift device in the sports environment it will be able to ring and emit a sound if movement is detected. It is equiped with a arduino chip, and other componants such as the movement sensor, a sim module with a 2g sim card, an anthenna, the buzzer and finally the battery. The lock will be able to be locked with an electro-magnet. 
You will find in this document all the specifications such as the voltage of each componant in the "" section.

## Deadlines

These deadlines were givin by Franck JEANNIN a stakeholder of the project. You will find the whole list of the stakeholders in the "" section.
- Functional 18/3 5pm
- Technical 26/3 5pm
- Test plan 10/4 5pm
- User Manual 10/4 5pm
- Code 10/4 5pm

## Materials

### Electronics
We were givin a prototype of the product to be able to work on it, Here is the specification of the componants that were givin by the client. 

|Image|Name|Dimensions|Description|Role|
|:-|:-|:-|:-|:-|
||Xiao BLE Sense nrf52840|2 x 2 x 0,5 cm | | Connects the USB C to the computer to import the code file.|
| |GNSS PA1010D | 2,5 x 2,5 x 1 cm | With antenna integration |This will allow to detect the movements of the board.
||GSM/2G SIM800L Module|2,2 x 1,8 x 0,5 cm | Sim card holder with 2G | This module will allow the board to connect to the 2G and send the location coordinates.
||Electromagnet|2,7 x 1,6 x 1,3 cm | 12V and 500mA electromagnet| This will allow to lock and unlock the system with the program.| 
||Piezoelectric buzzer|1,5cm diameter |12V with oscillaor circut control|This buzzer will allow to emit a sound ranging from 90db to 100db.
||Lithium-Polymer battery|5,1 x 3,5 x 0,6 cm | 3,7V 1100mAh and 4.1Wh lithium battery | Power source of the board and the electromagnet.|
||NFC antenna| 5,5 x 4,5 x 0,017cm|13,56Mhz frequency NFC antenna| This will allow the final user to use NFC technology to interact with the device.
|| USB type A to USB type C |10cm |10A connector| Will allow to connect for recharging and uploading code file.

These documents under was provided to our team to guide the team and for the team to understand the physical architecture of the board.

## Libaries

### Main libaries
- NRF52_MBED_TimerInterrupt V1.4.1
- ArduinoBLE v1.3.6
- Adafruit GPS Libary V1.7.4
- Sim800L http connector V1.14.0
- Seeed Arduino LSM6DS3 V2.0.3
- OneWire V2.3.7

### IDE
The working environnement for this project is Arduino IDE 2.3.2
"Link"




