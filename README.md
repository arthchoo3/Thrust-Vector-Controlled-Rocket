# Thrust-Vector-Controlled-Rocket

## General Overview
The rocket has an overall length of 490.75mm (19.32”), a diameter of 74.5mm (2.93”), and a total weight of 415g (14.64oz). It has four main sections: the nose cone, the avionics compartment, the main fuselage, and the thrust vector gimbals. The rocket is programmed to maintain a straight vertical trajectory by determining its orientation and correcting the direction of thrust accordingly. The rocket structure was designed in Fusion 360 and 3D printed with PLA, the PCBs were designed in EasyEDA and produced by JLCPCB, and the programming was typed and uploaded via the Arduino IDE. 

 ## Gimbals
 To control the direction of the thrust, the rocket uses a set of two gimbals which allows for rotation around two axes (one for roll and one for pitch). There is one SG90 Micro Servo to actuate each gimbal.
 ![Gimbal Picture](https://github.com/arthchoo3/Thrust-Vector-Controlled-Rocket/assets/140445967/1750c20b-d38a-422c-a0eb-c64b099e479b)
![Gimbal Picture 2](https://github.com/arthchoo3/Thrust-Vector-Controlled-Rocket/assets/140445967/289d0de0-176c-4b85-ac48-a0ef5eed17ff)


 ## Avionics
This avionics unit uses an ATmega328 microcontroller programmed with Arduino. It is powered by two 18650 lithium-ion batteries in series. Using an MPU-6050 gyroscope/potentiometer, the ATmega328 determines the rocket’s orientation and sends signals to the gimbal motors to adjust accordingly.
 ![Avionics Compartment](https://github.com/arthchoo3/Thrust-Vector-Controlled-Rocket/assets/140445967/93fc24c0-f2da-45a0-9601-28816c78e207)

