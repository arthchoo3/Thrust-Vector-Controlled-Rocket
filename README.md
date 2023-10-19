# Thrust-Vector-Controlled-Rocket
This repository contains the design process of my thrust vector-controlled rocket, including the STL, Gerber, and Ino files.

## General Overview
The rocket has an overall length of 490.75mm (19.32”), a diameter of 74.5mm (2.93”), and a total weight of 415g (14.64oz). It has four main sections: the nose cone, the avionics compartment, the main fuselage, and the thrust vector gimbals. The rocket is programmed to maintain a straight vertical trajectory by determining its orientation and correcting the direction of thrust accordingly. The rocket structure was designed in Fusion 360 and 3D printed with PLA, the PCBs were designed in EasyEDA and produced by JLCPCB, and the programming was typed and uploaded via the Arduino IDE. 

 ## Gimbals
 To control the direction of the thrust, the rocket uses a set of two gimbals which allows for rotation around two axes (one for roll and one for pitch). There is one SG90 Micro Servo to actuate each gimbal.

 ## Avionics
This avionics unit uses an ATmega328 microcontroller programmed with Arduino. It is powered by two 18650 lithium-ion batteries in series which produce a total of 7.4 volts, a battery eliminator circuit then drops this voltage to the operational 5 volts. Using an MPU-6050 gyroscope/potentiometer, the ATmega328 determines the rocket’s orientation and sends signals to the gimbal motors to adjust accordingly.
 
