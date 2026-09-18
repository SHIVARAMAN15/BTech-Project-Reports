# 🤖 Smart Patrol Bot

## 📌 Project Overview

The **Smart Patrol Bot** is an autonomous mobile surveillance robot designed for indoor security applications. The system combines motion detection, wireless communication, live video monitoring, and mobile robotic control using low-cost embedded hardware.

The project was developed as part of **Project Exhibition–II** for the B.Tech program in **Electronics and Communication Engineering (AI & Cybernetics)** at **VIT Bhopal University**.

The robot is designed to:

- Detect human motion
- Patrol an indoor environment
- Stream live video
- Capture images during detected activity
- Provide remote monitoring
- Send alerts to the user

---

## 🎯 Key Features

- 🔍 **Motion Detection** using PIR sensors
- 📷 **Live Video Streaming** using ESP32-CAM
- 📸 **Image Capture** during detected activity
- 🤖 **Mobile Robotic Navigation** using DC motors
- ⚙️ **Motor Control** using L298N motor driver
- 📡 **Wireless Communication** using Wi-Fi and Bluetooth
- 📲 **Remote Monitoring** through connected interfaces
- 🚨 **Alert System** using Telegram
- 🧠 **Software-Based Detection** using Python and Flask

---

## 🛠️ Hardware Components

| Component | Description |
|-----------|-------------|
| ESP32-CAM | Camera module with Wi-Fi and Bluetooth connectivity |
| Arduino UNO | Motor and sensor control |
| L298N | Dual H-Bridge motor driver |
| PIR Sensor | Human motion detection |
| HC-05 | Bluetooth communication |
| DC Gear Motors | Robot movement |
| FTDI Module | ESP32-CAM programming |
| Battery | Portable power supply |

---

## 🧠 System Architecture

```text
                 ┌─────────────────────┐
                 │    PIR Sensors      │
                 │  Motion Detection   │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │     Arduino UNO     │
                 │ Sensor & Motor      │
                 │ Control             │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │    L298N Driver     │
                 └──────────┬──────────┘
                            │
                            ▼
                 ┌─────────────────────┐
                 │    DC Gear Motors   │
                 │ Robot Movement      │
                 └─────────────────────┘


                 ┌─────────────────────┐
                 │      ESP32-CAM      │
                 │ Camera + Wi-Fi      │
                 └──────────┬──────────┘
                            │
                    ┌───────┴────────┐
                    ▼                ▼
             Live Video         Image Capture
                    │                │
                    └───────┬────────┘
                            ▼
                 ┌─────────────────────┐
                 │ Remote Monitoring   │
                 │ / Telegram Alerts   │
                 └─────────────────────┘
