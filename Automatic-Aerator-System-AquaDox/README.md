# 🌊 Automatic Aerator System – AquaDox

### Project Proposed for Project Exhibition – I
**VIT Bhopal University**

---

## 📌 Project Overview

**AquaDox** is an automatic aeration system designed for **aquaculture environments** to maintain suitable dissolved oxygen levels in water.

The system continuously monitors important water parameters and automatically controls the aerator based on the measured dissolved oxygen level. This reduces the need for continuous manual monitoring and helps maintain a healthier environment for aquatic organisms.

The project combines **embedded systems, sensors, automation, and IoT-based monitoring** to provide an efficient and practical aquaculture solution.

---

## 🎯 Objectives

- Monitor dissolved oxygen levels in real time.
- Automatically control the aerator based on oxygen-level thresholds.
- Monitor important water-quality parameters.
- Reduce unnecessary aerator operation and energy consumption.
- Provide remote monitoring and system-status information.
- Improve reliability of aquaculture water management.

---

## ✨ Key Features

- 📡 **Real-Time Monitoring**  
  Continuously monitors dissolved oxygen and other water parameters.

- ⚡ **Automatic Aeration**  
  Automatically switches the aerator ON/OFF based on configured threshold values.

- 🌡️ **Water Temperature Monitoring**  
  Monitors water temperature for improved water-quality assessment.

- 📱 **Remote Monitoring**  
  Provides remote access to system status through the connected monitoring interface.

- 🌞 **Energy-Efficient Operation**  
  Aeration is activated according to the required oxygen conditions instead of running continuously.

- 🔔 **Alerts & Notifications**  
  Provides notifications when monitored parameters reach critical conditions.

---

## 🧠 System Working Principle

```text
        ┌──────────────────────┐
        │   Water Environment  │
        └──────────┬───────────┘
                   │
                   ▼
        ┌──────────────────────┐
        │   Sensor Module      │
        │                      │
        │ Dissolved Oxygen     │
        │ Temperature          │
        │ pH / Other Sensors   │
        └──────────┬───────────┘
                   │
                   ▼
        ┌──────────────────────┐
        │   Microcontroller    │
        │                      │
        │ Sensor Processing    │
        │ Threshold Analysis   │
        │ Control Logic        │
        └──────────┬───────────┘
                   │
                   ▼
        ┌──────────────────────┐
        │   Relay / Driver     │
        └──────────┬───────────┘
                   │
                   ▼
        ┌──────────────────────┐
        │       Aerator        │
        │                      │
        │  Oxygen Generation   │
        └──────────────────────┘

                   │
                   ▼
        ┌──────────────────────┐
        │ Monitoring Interface │
        │ / IoT Dashboard      │
        └──────────────────────┘
