# Arduino Obstacle Avoidance Robot 🤖

This repository contains the source code and circuit details for an autonomous Obstacle Avoidance Robot built using an Arduino UNO and an Ultrasonic Sensor.

## 🛠️ Components Used
* Arduino UNO
* HC-SR04 Ultrasonic Sensor
* L298N Motor Driver
* 2x DC Gear (BO) Motors and Wheels
* 1x Caster Wheel
* Robot Chassis
* 9V or 12V Battery & Jumper Wires

## 🔌 Circuit Connections

**Ultrasonic Sensor:**
* VCC -> Arduino 5V
* GND -> Arduino GND
* TRIG -> Arduino Analog Pin A0
* ECHO -> Arduino Analog Pin A1

**Motor Driver (L298N):**
* IN1, IN2, IN3, IN4 -> Arduino Pins 8, 9, 10, 11
* 12V -> Battery Positive (+)
* GND -> Battery Negative (-) AND Arduino GND
* 5V -> Arduino VIN

## 🚀 How it Works
1. The HC-SR04 sensor sends out a sound wave and listens for the echo.
2. The Arduino calculates the distance to the nearest object in front of the robot.
3. If the distance is less than 20 cm, the robot stops, moves backward slightly, and turns right to find a clear path.
4. If the path is clear (distance > 20 cm), it keeps moving forward.

## 👨‍💻 How to Use
1. Download or clone this repository.
2. Open `obstacle_avoider.ino` in the Arduino IDE.
3. Compile and upload it to your Arduino UNO.
