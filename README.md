This is an autonomous robot that follows a black line on a white surface using infrared (IR) sensors. It is built on an Arduino Uno platform and uses two DC motors with a motor driver for movement. The robot detects the line using IR sensors and adjusts its direction accordingly.

1.Line-Following Arduino Robot on the line

2.Description
This project is an autonomous robot that follows a black line on a white surface using infrared (IR) sensors. It is based on the Arduino Nano and is designed to demonstrate basic robotics, sensor integration, and motor control. The robot uses simple logic to stay on the path by constantly adjusting its direction based on input from eight IR sensors.
3.Components Used
- Arduino Nano
- 2x Motors(G12-N20 9V) with wheels
- 8 sensor lines follow
- Tracker Sensor V2.1
- Engine driver TB6612FNG
- 7.4-9V Battery or Power Bank

4.How It Works
The robot uses an 8-channel infrared sensor array to detect a black line on a white surface.
Each channel (sensor) sends a signal to the Arduino indicating whether it detects black (low reflection) or white (high reflection).
The sensor array gives the robot a more detailed view of the line’s position, allowing it to make smoother and more accurate movements.
The Arduino reads the digital (or analog) values from all 8 sensors and determines the line’s position relative to the center of the robot.
Based on which sensors detect the line, the robot adjusts the speed of its left and right motors:
If the line is in the center, both motors move forward.
If the line shifts left or right, the robot slows one motor and speeds up the other to realign.     

6.Instructions:
1.Assemble the robot chassis and attach all components.
2.Connect the motors to the TB6612FNG motor driver.
3.Connect IR sensors to the digital pins of Arduino.
4.Connect Motor driver to Arduino (BIN1,BIN2,VCC,GND,AIN1,AIN2, PWMA,PWMB).
5.Upload the Arduino sketch from the code/ folder.
6.Place the robot on a black line and turn it on.

7.Photos
![Arduino Robot1](https://github.com/Akez76/Arduino-Robot/blob/main/hgl06ktw.png)
![Arduino Robot2](https://github.com//Akez76/Arduino-Robot/blob/main/robot2.jpeg)



8.Skills Used
-Arduino programming (C++)
-Sensor input handling
-Motor control (PWM)
-Autonomous movement logic

Author:
Akezhan Kurbanov




