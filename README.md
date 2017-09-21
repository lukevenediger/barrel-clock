# barrel-clock
An internet-connected clock driven by Arduino and ESP8288

# Basic Idea
I'm really fascinated by analog clocks and analog data displays in general. I feel like they are usually
great at conveying single data points. In other words, they work well doing just one job.

This clock will display hours and minutes using three rotors:
* First rotor will be for the HOURS value
* Second and third rotor will be grouped to show the MINUTES value

# Hardware

## Mechanism Design
The clock mechanism has been designed in Tinkercad (see: https://www.tinkercad.com). https://www.tinkercad.com/things/lrkl3aIcL03-barrel-rotor

## Components
* Arduino Nano - to control the motors and will hold core logic
* ESP-8266 (ESP-01) - to enable wifi capabilities for the clock
* OR a bluetooth module, that will allow configuration using an app
* DS1402 RTC - to maintain the internal clock (requires a battery)
* UV LED - one per rotor
* 28BYJ-48 Stepper Motors
* ULN2003 darlington array
* 8-bit Shift Registers (74HC595)

# Software
