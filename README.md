# Line-Following Robot

## Overview
This project demonstrates an **Arduino-based line-following robot** designed to autonomously follow a predefined path using **IR sensors** and a **motor driver (L298N)**. It provides a low-cost, beginner-friendly solution for learning embedded systems, automation, and robotics.

The robot detects black lines on a white surface and adjusts its movement in real-time, making it suitable for educational purposes, prototyping, and small-scale automation.

## Features
- Autonomous navigation using IR sensors.
- Arduino Uno microcontroller as the central processing unit.
- L298N motor driver for bidirectional DC motor control.
- Modular and expandable design for future enhancements (e.g., obstacle avoidance, wireless control).

## Components
- **Arduino Uno R3**: Central microcontroller for processing sensor input and controlling motors.
- **IR Sensors (Left & Right)**: Detect line using infrared reflection (HIGH for white, LOW for black).
- **L298N Motor Driver**: Controls direction and speed of two DC motors.
- **DC Motors**: Provides mobility and directional control.
- **Power Supply**: 9V battery or USB connection.

## Block Diagram
![Block Diagram](6476ec9a-1955-47b1-b0ad-85befd17af58.png)

## Working Principle
1. IR sensors detect the surface reflectivity (white reflects IR, black absorbs IR).
2. Arduino processes sensor input and determines motor direction:
   - Both sensors detect white → move forward.
   - Left sensor detects black → turn left.
   - Right sensor detects black → turn right.
   - Both detect black → stop or reverse.
3. Motor driver executes Arduino commands to move the robot along the line.

## Methodology
- Prototype assembled on a breadboard to test sensors and motor control.
- Programmed using **Arduino IDE** with simple conditional logic.
- Tested on straight lines, curves, and intersections to evaluate performance.
- Final assembly on chassis with sensor placement adjustments for optimal tracking.

## Results
- **Accuracy**: ~93% line detection on clean paths.
- **Response Time**: <100ms for directional adjustments.
- **Battery Life**: ~1.5 hours with 9V battery.
- Smooth navigation on straight and curved paths.
- Low-cost and reliable for educational and prototyping purposes.

## Future Work
- Obstacle avoidance using ultrasonic or IR proximity sensors.
- Implement PID control for precise turning.
- Wireless control via Bluetooth, Wi-Fi, or RF modules.
- IoT integration for data logging and monitoring.
- Advanced line following using camera and image processing.
- Motor speed control with encoders for smoother movement.

