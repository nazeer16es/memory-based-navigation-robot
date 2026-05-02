
---

## Memory-Based Navigation Robot (ESP32)

## Project Presentation

View PPT: [https://canva.link/zyxfwo3kz4fpoq7](https://canva.link/zyxfwo3kz4fpoq7)

---

## Project report

View report: .[report](https://github.com/nazeer16es/memory-based-navigation-robot/blob/main/memory-based-navigation-robot-report.pdf)

## Overview

This project implements a memory-based navigation robot using an ESP32 microcontroller. The robot is capable of learning a path through manual control and later repeating the same path autonomously without user intervention.

The system uses motor encoders to record movement data such as distance and direction, which is then stored and replayed for autonomous navigation.

---

## Features

* Path learning through manual control
* Autonomous path replay
* Encoder-based distance and speed measurement
* Bluetooth-based mobile control
* Data storage for navigation replay

---

## Working Principle

### Learning Phase

* The robot is controlled manually using a Bluetooth mobile application
* Wheel encoders generate pulses during movement
* ESP32 records encoder data (distance and direction)
* Movement data is stored in memory

---

### Autonomous Phase

* Stored movement data is retrieved
* Robot replays the recorded path
* Encoder feedback ensures accurate motion replication

---

### Encoder-Based Control

* Encoders generate pulses proportional to wheel rotation
* ESP32 counts pulses to calculate:

  * Distance traveled
  * Speed of movement
* Enables controlled and repeatable navigation

---

## Core Functionality

* Motor control using motor driver
* Encoder interfacing and pulse counting
* Bluetooth communication for manual control
* Memory storage and retrieval of path data
* Autonomous motion execution

---

## Components Used

* ESP32 Development Board
* Motor Driver (L298N or similar)
* DC Motors with Encoders
* Battery Supply
* Bluetooth Mobile Application

---

## Applications

* Path-following robots
* Warehouse automation
* Delivery robots
* Educational robotics systems

---

## Limitations

* No obstacle detection mechanism
* Performance affected by wheel slipping
* No feedback correction (no PID control)
* Accuracy depends on surface conditions

---

## Possible Improvements

* Add ultrasonic or IR sensors for obstacle avoidance
* Implement PID control for precise movement
* Use IMU or additional sensors for better accuracy
* Add real-time path correction
* Store data in non-volatile memory

---

## Conclusion

This project demonstrates encoder-based navigation, data-driven path learning, and autonomous motion control using ESP32. It provides a foundation for building advanced autonomous robotic systems.

---
