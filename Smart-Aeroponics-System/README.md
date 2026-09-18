# 🌱 Smart Aeroponics System

An IoT-enabled, automated aeroponics platform integrating ESP32-based sensing and control, real-time wireless telemetry, automated nutrient dosing, ultrasonic mist generation, safety mechanisms, and local AI-assisted analytics.

---

## 📌 Project Overview

The **Smart Aeroponics System** is an engineering project developed for soilless cultivation using a nutrient-rich mist delivered directly to plant roots.

The system combines:

- ESP32-based embedded control
- Multi-sensor data acquisition
- Signal filtering and calibration
- Closed-loop nutrient and pH control
- Ultrasonic nebulizer-based mist generation
- Automated low-water safety shutdown
- Wi-Fi-based telemetry
- Telegram Bot remote monitoring
- Streamlit dashboard
- Local JSON data storage
- Local AI-assisted analysis using Ollama and Llama 3.2
- Automated TXT and PDF reporting

The system is designed for controlled, automated, and data-driven aeroponic cultivation.

---

## 🚀 Key Features

### 🌱 Aeroponic Cultivation

- Soil-less plant cultivation
- Nutrient-rich mist delivery
- Exposed root-zone environment
- Ultrasonic nebulizer-based mist generation
- Timed misting control

### 📡 IoT Monitoring

- ESP32-based wireless connectivity
- Real-time sensor data acquisition
- Wi-Fi telemetry
- Telegram Bot monitoring
- Remote alerts and notifications
- HTTP-based control interface

### ⚗️ Sensor Monitoring

The system monitors important environmental and nutrient-solution parameters:

- pH
- TDS / EC
- Temperature
- Humidity
- Water Level

### 🔄 Automated Control

- Closed-loop pH control
- Automated pH-Up dosing
- Automated pH-Down dosing
- Automated nutrient dosing
- Incremental dosing pulses
- Automated misting cycles
- Low-water safety shutdown

### 🤖 Local AI / ML Intelligence

- Local AI processing
- Trend analysis
- Anomaly detection
- Predictive insights
- pH drift analysis
- Nutrient depletion analysis
- Natural-language interaction with historical data
- Retrieval-Augmented Generation (RAG)

### 📊 Dashboard and Reporting

- Streamlit dashboard
- Real-time metric visualization
- Time-series trend analysis
- Interactive AI assistant
- Password-protected dashboard
- Automated TXT reports
- On-demand PDF reports
- Historical data analysis

---

# 🧠 System Architecture

The system follows a hybrid hardware-software architecture consisting of sensing, control, communication, data processing, intelligence, visualization, and reporting layers.

```text
                    ┌───────────────────────────┐
                    │       SENSOR LAYER        │
                    │                           │
                    │ pH | TDS/EC | Temperature │
                    │ Humidity | Water Level    │
                    └─────────────┬─────────────┘
                                  │
                                  ▼
                    ┌───────────────────────────┐
                    │      ESP32 CONTROLLER     │
                    │                           │
                    │ Data Acquisition          │
                    │ Signal Filtering          │
                    │ Calibration               │
                    │ Control Logic             │
                    │ Safety Logic              │
                    └─────────────┬─────────────┘
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
                    ▼                           ▼
          ┌──────────────────┐       ┌──────────────────┐
          │   ACTUATOR LAYER │       │ COMMUNICATION    │
          │                  │       │      LAYER       │
          │ Peristaltic      │       │ Wi-Fi            │
          │ Pumps            │       │ Telegram Bot     │
          │                  │       │ HTTP             │
          │ Ultrasonic       │       └────────┬─────────┘
          │ Nebulizer        │                │
          └──────────────────┘                ▼
                                    ┌──────────────────┐
                                    │ DATA PROCESSING  │
                                    │                  │
                                    │ JSON Storage     │
                                    │ Data Parsing     │
                                    └────────┬─────────┘
                                             │
                                             ▼
                                    ┌──────────────────┐
                                    │   AI LAYER       │
                                    │                  │
                                    │ Ollama           │
                                    │ Llama 3.2        │
                                    │ RAG              │
                                    │ Anomaly Detection│
                                    └────────┬─────────┘
                                             │
                                             ▼
                                    ┌──────────────────┐
                                    │ APPLICATION      │
                                    │     LAYER        │
                                    │                  │
                                    │ Streamlit        │
                                    │ Dashboard        │
                                    │ AI Assistant     │
                                    └────────┬─────────┘
                                             │
                                             ▼
                                    ┌──────────────────┐
                                    │ REPORTING LAYER  │
                                    │                  │
                                    │ TXT Reports      │
                                    │ PDF Reports      │
                                    └──────────────────┘
