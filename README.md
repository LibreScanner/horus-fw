# Horus 3D Scanner Firmware

Modified from the original firmware by Gyrobot to work with the Arduino UNO and CNC V3 Shield.

* Motor is driven by "X" Pololu driver.
* 12V power supply <1A to CNC V3 shield required for motor.
* Lasers are fired by "Z.STEP and Z DIR" pins.

This firmware is written in C.

Derived from Grbl v0.9 by Jesús Arroyo (Mundo Reader S.L.)

Grbl's lead developer is Simen Svale Skogsrud. Sonney Jeon (Chamnit) improved some parts of grbl.


## Features

*   Angular stepper motor movement
*   Interrupt based movement with real angular acceleration
*   Laser modules control
*   Analog sensor read
*   Configuration interface with $ commands

The default baudrate is 115200.


## Implemented G Codes

*   G1  - Circular movement
*   M0   - Program pause
*   M2   - Program end and reset
*   M17  - Enable/Power stepper motor
*   M18  - Disable stepper motor
*   M50  - Read LDR
*   M70  - Laser off
*   M71  - Laser on