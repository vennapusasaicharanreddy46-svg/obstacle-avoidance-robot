# 🤖 Obstacle Avoidance Robot

> An autonomous robotic vehicle that detects and avoids obstacles using an ultrasonic sensor.

---

## 📌 Overview

The Obstacle Avoidance Robot is an autonomous robotic system designed to move without human control while avoiding collisions. The robot uses an ultrasonic sensor to detect obstacles in its path and automatically changes direction to prevent crashes.

This project demonstrates embedded systems, sensor interfacing, motor control, and real-time autonomous decision-making.

---

## ✨ Features

* 🚗 Fully autonomous movement
* 📏 Real-time distance measurement
* 🛑 Automatic obstacle detection
* 🔄 Self-direction control (Left/Right/Back)
* 🔋 Battery-powered and portable
* 🔧 Expandable for advanced robotics

---

## 🛠️ Hardware Components

* Arduino Uno / Nano
* HC-SR04 Ultrasonic Sensor
* L298N Motor Driver Module
* DC Motors (2 or 4)
* Robot Chassis
* Servo Motor (optional for scanning)
* Battery Pack
* Jumper Wires

---

## ⚙️ Working Principle

1. The ultrasonic sensor continuously sends ultrasonic waves.
2. When the waves hit an obstacle, they reflect back.
3. The sensor calculates the distance based on echo time.
4. The Arduino reads the distance value.
5. If the distance is safe, the robot moves forward.
6. If an obstacle is detected within a threshold (e.g., 20 cm), the robot stops and changes direction.

If a servo motor is used, the sensor rotates left and right to scan the surroundings before choosing the best path.

---

## 🔄 Movement Logic

| Condition        | Action          |
| ---------------- | --------------- |
| Distance > 20 cm | Move Forward    |
| Distance < 20 cm | Stop            |
| Obstacle Ahead   | Turn Left/Right |
| No Clear Path    | Move Backward   |

---

## 🚀 How to Run

1. Install Arduino IDE.
2. Connect Arduino board.
3. Upload the obstacle avoidance code.
4. Connect motors via L298N motor driver.
5. Power the robot.
6. Place the robot on the ground — it will move autonomously.

---

## 📂 Project Structure

```
Obstacle-Avoidance-Robot/
│
├── code/
│   └── obstacle_robot.ino
├── images/
├── circuit/
└── README.md
```

---

## 🔮 Future Improvements

* Add Bluetooth / WiFi control
* Add camera for smart vision navigation
* AI-based path planning
* GPS-based outdoor navigation
* Edge detection using IR sensors

---

## 📌 Applications

* Warehouse automation
* Industrial robots
* Smart cleaning robots
* Military surveillance
* Disaster management

