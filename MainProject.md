# Automatic-Water-Level-Controller-using-Arduino-Ultrasonic-Sensor
This project is a smart water level controller built using Arduino UNO, an ultrasonic sensor, and EEPROM for memory storage. The system automatically monitors the water level in a tank and controls the motor (pump) based on the percentage of water present.

**Abstract :**


This project presents the design and implementation of an Automatic Water Level Controller using an Arduino UNO and an ultrasonic sensor. The system monitors the water level in a tank in real-time and automatically controls a water pump based on predefined threshold values. The ultrasonic sensor measures the distance to the water surface, and the data is processed to calculate the water level percentage. The Arduino activates or deactivates the pump accordingly, ensuring efficient water usage and preventing overflow. A user-defined maximum tank level can be set and stored in the EEPROM for future use. Manual override functionality is also integrated for pump control and calibration. This project is cost-effective, energy-efficient, and suitable for residential and agricultural water management applications.

**Simulation and Design :**

![image]![image](https://github.com/user-attachments/assets/7161477d-26e5-46a7-b173-a78881119c2f)



This project demonstrates an Automatic Water Level Controller using an Arduino Uno, HC-SR04 ultrasonic sensor, a relay module, and two push buttons. The ultrasonic sensor measures the distance from the sensor to the water surface, which is then used to calculate the water level as a percentage. Based on this value, the Arduino decides whether to turn the water pump ON or OFF. The pump is controlled using a 5V relay module, which acts as a switch connected to pin 12 of the Arduino.

The wiring in the diagram shows the ultrasonic sensor's trigger and echo pins connected to pins 8 and 9 respectively. Two push buttons are used: one for calibration (setting the maximum water level) and another for manual override of the motor. These are connected to pins 10 and 11 with pull-up resistors. The system reads the ultrasonic values, computes the percentage of the water level relative to the set maximum, and activates the pump when the level falls below 95%. When the tank fills to 99%, the pump is turned off automatically.

The EEPROM is used to store the maximum distance (set by the user) so the system remembers it even after power is lost. The serial monitor displays the water percentage and pump status for debugging and monitoring. This project is highly useful for automating household or ag
