# 🚗 Basic Robot Car Command — Arduino Autonomous Navigation Project
This repository contains the **Basic Robot Car Command system**, developed as an Arduino project focusing on **autonomous navigation and obstacle avoidance**. 
The robot car uses **ultrasonic sensors, a servo motor for directional scanning**, and a **PID control algorithm** to dynamically detect obstacles and choose the safest path forward. 
The system allows the car to move forward, reverse, or make precise turns to navigate around obstacles without human intervention.
<br><br>

### 📦 Technologies & Components Used
**Hardware**
- Arduino Uno (or compatible microcontroller)
- L298N Motor Driver
- Ultrasonic Distance Sensor (HC-SR04)
- Servo Motor (for directional scanning)
- DC Motors (Left and Right drive)
- Power supply (Battery pack)

**Software & Libraries**
- Servo.h — Controls the servo motor for scanning
- PID_v1.h — Implements PID control for navigation adjustments
- Arduino IDE — Development environment
<br><br>

### ⚙️ Project Features
- **Autonomous Navigation:** The car automatically moves forward and adjusts its path when obstacles are detected.
- **Obstacle Avoidance:** Uses ultrasonic sensors to detect distances and make decisions in real time.
- **Servo-Based Scanning:** Dynamically rotates the ultrasonic sensor left and right to check for clear paths.
- **PID Control:** Helps maintain stable and responsive movement decisions based on sensor readings.
- **Fallback Behavior:** If both directions are blocked, the car reverses until a safe path is available.
<br><br>

### 📊 System Workflow
- **Forward Movement:** The car moves forward as long as no obstacles are detected within the set threshold (30 cm).
- **Obstacle Detection:** When an obstacle is detected, the car stops and scans left and right.
- **Path Selection:** The robot chooses the direction with more available space.
- **Dynamic Turning:** The car turns toward the selected direction until the path is clear.
- **Resume Movement:** Once a clear path is available, it continues moving forward.
