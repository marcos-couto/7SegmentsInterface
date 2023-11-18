# Display 7 Segment interface
## Project Description: 
7-Segment Display with 74HC595, ULN2803A, and SPI Interface
![Interface Board](/Images/ASTDC01V01.png "Interface Board")
![B Board](/Images/BBoard.png "B Board")
![F Board](/Images/FBoard.png "F Board")

## Overview:
This project aims to create a simple yet effective interface for a 7-segment display using common components like the 74HC595 shift register, ULN2803A darlington array, and SPI communication with a microcontroller. The combination of these components allows for efficient control of the 7-segment display using minimal pins on the microcontroller.


## Components:
- 7-segment display (common cathode)
- 74HC595 shift register
- ULN2803A darlington array
- Microcontroller with SPI capabilities 

## Connections:

- Connect the common cathode of the 7-segment display to GND.
- Connect the anode pins of each segment to the corresponding output pins of the ULN2803A.
-  Connect the input pins of the ULN2803A to the output pins of the 74HC595 shift register.
- Connect the serial data input (DS), shift register clock (SH_CP), and storage register clock (ST_CP) of the 74HC595 to the MOSI, SCK, and SS pins of the microcontroller, respectively.
- Connect the Output Enable (OE) pin of the ULN2803A to a digital pin on the microcontroller

## Basic Operation:
The microcontroller sends data to the 74HC595 shift register using SPI communication. The shift register outputs are then connected to the input pins of the ULN2803A, which in turn controls the segments of the 7-segment display. The Output Enable (OE) pin of the ULN2803A is used to enable or disable the display, providing control over when the display is active.

