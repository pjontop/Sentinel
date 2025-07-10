---
title: "Sentinel"
author: "Pramsu Pandey"
description: "A fully autonomous, AI-powered drone with VR compatibility and a DJI-style controller for immersive, intelligent flight."
created_at: "2024-03-20"
---

# Vision - 1:30hr

I’ve been searching around for about an hour and here are some requirements I wanna tick off for this project.

## Hardware Requirements

### Flight Controller PCB
- Custom Designed with a barometer compass, PWM outputs, and regulated power

### Motors and ESCs
- 4x brushless motors

### Frame
- Custom CAD Aluminum frame with airflow and mounting

### Battery
- 3000-5000 mAh capacity

### Power Distribution
- Integrated PCB with high current copper pours

### Sensors
- GPS (like the u-blox NEO-M8N)
- Ultrasonic or LiDar (for obstacle avoidance)

### Camera
- Stereoscopic or 360 VR-Capable camera module
- Low latency and streaming

### Companion Computer
- RPI 5 for AI tasks, SLAM and vision

### Wireless Comms
- 5GHz wifi for video + telemetry
- Long-range 2.4GHz or 915 MHz for control

## Software Requirements

### Onboard software
- Realtime flight firmware running on MCU
- Auton logic and SLAM on companion compute (RP2040?)
- AI Obj recognition using tensor models
- MAVLink for control and telemetry
- VR Video streaming (low latency maybe web RTC w/ a SIM card / cellular functionality)

### Ground Station
- Custom UI dashboard: live map, telemetry, controls and camera feed
- VR support

### Safety + Reliability
- Redundant IMU
- Auto landing on critical battery
- Fail safe hover
- Signal integrity and watchdog timers on control links
- GPS geofencing w/ NFZ

## Functional Requirements

- Should be able to fly autonomously using onboard AI and sensor data
- The drone should support real-time VR video streaming to a head (like the Quest)
- It should be controlled via my keyboard and trackpad
- It should be able to detect and avoid obstacles
- It should be able to return-to home in real time
- It should operate in a 1-3 km range

# Ideas
