# LEDMatrix
Making Led matrix using arduino
INTRODUCTION

In this project, we will learn about LED Matrix Displays and two different projects on Arduino 8×8 LED Matrix Interface. The project will be a simple interface between Arduino and 8X8 LED Matrix to display information (even scrolling information and images can be displayed). An LED matrix is a two dimensional array of LEDs that can be used to display symbols, characters or even images.
Based on the orientation of the LEDs in the matrix, there can be two types of LED matrices. They are Common Row Anode and Common Row Cathode. The aim of the project is to interface an Arduino Uno board with an 8 x 8 LED matrix to display information. Even though a single 8 x 8 LED matrix with corresponding MAX 7219 IC is used in this project, multiple LED matrices can be connected in series for long scrolling display.

MOTIVATION

It is needed to show the texts or images in public places for better visual understanding and better communication. For example in today’s world it is used in traffic lights, malls and shopping complexes, public transportation like buses & metro and in widely many more areas.

METHODOLOGY

To make a project where we will be using different hardware components for displaying images and text on the matrix LED’s. We will be using LED matrix, Arduino UNO, Breadboard, some IC’s and wires. It will be a IOT project where we will be connecting all hardware components and then with the help of some simple program of Arduino UNO, we will be displaying graphics on the matrix
LED’s. 3 of the 14 available digital input / output pins are used to control the display driver IC MAX 7219. The 3 pins on the MAX7219 IC are clock, data in and load (or cs in case of MAX 7221 IC). A maximum clock frequency of 10MHz can be applied. DIN (Data in) accepts the serial data from the microcontroller or Arduino board. It is 16 bit long where the first 8 bits (D0 – D7) are for driving the columns (SEG A-G and DP of the MAX 7219 IC) of the LED matrix and the next 8 bits (D8 – D15) are for driving the (DIG 0-7 of the MAX 7219 IC) rows of the LED matrix. The load pin (or CS or chip select pin in case of Max 7221 IC) latches the serial input data on its rising edge.
Another important pin on MAX 7219 is the ISET, which sets the peak current to the segment to drive all the LEDs. It is connected via a resistor (R1), which is called RSET. The capacitors filters
 
out any noise in the supply. When the serial data in is sent using the Arduino (through the program), the serial data is converted into segments and digits to drive columns and rows of the LED matrix. According to the data sent, the corresponding LEDs on the matrix light up and display the message. The program written here is for scrolling text display. It might be difficult to view long scrolling data on a single 8 x 8 LED matrix. Hence, multiple LED matrices can be chained to form a long matrix. The no. of MAX 7219 ICs are equal to the no. of 8 x 8 LED matrices. In order to extend the display to multiple LED matrices, the Data OUT (DOUT) pin of the first MAX 7219 must be connected to the Data IN (DIN) pin of the second MAX 7219 IC. This process must be continued for multiple LED matrices.
 

TECHNOLOGIES USED


1.	Arduino Uno board - The project is based on the Arduino Uno microcontroller board. Out of the 14 available digital input / output pins on the Arduino Uno, we need only three pins to implement this project.
2.	LED Matrix – 8 x 8 LED dot matrix - An 8 x 8 LED matrix display is used in this project to display the information. LED matrices are available in different styles like single color, dual color, multi-color or RGB LED matrix.
3.	IC1 – MAX 7219 - MAX 7219 is a common cathode display driver with serial input and parallel output. It is used to interface microprocessors and microcontrollers with 64 individual LEDs (8 x 8 LED matrix for example has 64 LEDs), seven segment LED displays up to 8 digits or bar graph
 
displays.
4. R1 – 10 KΩ
5. C1 – 0.1 μF
6. C2 – 10 μF
7.	Arduino IDE

