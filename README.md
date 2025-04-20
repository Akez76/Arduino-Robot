This is an autonomous robot that follows a black line on a white surface using infrared (IR) sensors. It is built on an Arduino Uno platform and uses two DC motors with a motor driver for movement. The robot detects the line using IR sensors and adjusts its direction accordingly.

# 1.Description
This project is based on the Arduino Nano and is designed to demonstrate basic robotics, sensor integration, and motor control. The robot uses simple logic to stay on the path by constantly adjusting its direction based on input from eight IR sensors.

# 2.Components Used
- Arduino Nano
- 2x Motors(G12-N20 9V) with wheels
- 8 sensor lines follow
- Tracker Sensor V2.1
- Engine driver TB6612FNG
- 7.4-9V Battery or Power Bank


# 3.How It Works
The robot uses an 8-channel infrared sensor array to detect a black line on a white surface.
Each channel (sensor) sends a signal to the Arduino indicating whether it detects black (low reflection) or white (high reflection).
The sensor array gives the robot a more detailed view of the line’s position, allowing it to make smoother and more accurate movements.
The Arduino reads the digital (or analog) values from all 8 sensors and determines the line’s position relative to the center of the robot.
Based on which sensors detect the line, the robot adjusts the speed of its left and right motors:
If the line is in the center, both motors move forward.
If the line shifts left or right, the robot slows one motor and speeds up the other to realign.     


# 4.Instructions:
- Assemble the robot chassis and attach all components.
- Connect the motors to the TB6612FNG motor driver.
- Connect IR sensors to the digital pins of Arduino.
- Connect Motor driver to Arduino (BIN1,BIN2,VCC,GND,AIN1,AIN2, PWMA,PWMB).
- Upload the Arduino sketch from the code/ folder.
- Place the robot on a black line and turn it on.

# 5.Wiring Summary
| Component                | Arduino Pin |
|--------------------------|-------------|
| TB6612FNG PWMA           | D11         |
| TB6612FNG PWMB           | D10         |
| TB6612FNG AIN1           | D7          |
| TB6612FNG AIN2           | D8          |
| TB6612FNG BIN1           | D6          |
| TB6612FNG BIN2           | D5          |
| TB6612FNG VCC            | 5V          |
| TB6612FNG GND            | GND         |
| Tracker Sensor V2.1 OTL  | D2          |
| Tracker Sensor V2.1 OTC  | D3          |
| Tracker Sensor V2.1 OTR  | D4          |
  

# 6.Photos
![Arduino Robot1](https://github.com/Akez76/Arduino-Robot/blob/main/hgl06ktw.png)
![Arduino Robot2](https://github.com//Akez76/Arduino-Robot/blob/main/robot2.jpeg)


# 7.Skills Used:
- Arduino programming (C++)
- Sensor input handling
- Motor control (PWM)
- Autonomous movement logic



# Author:
Akezhan Kurbanov
