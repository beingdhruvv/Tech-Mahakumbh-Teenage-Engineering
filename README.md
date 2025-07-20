# ⚡ Intelligent Energy Management System (IEMS)

**Team:** Teenage Engineering Works  
**Team Members:** Dhruv Suthar, Pratham Patel, Hena Patel  
**Version:** 4.1 (Updated: 7 July 2025)

---

![IEMS DEMO VIDEO](https://github.com/user-attachments/assets/54c72df2-a1fb-4397-b787-678a62b644d6)
![System Setup](https://github.com/user-attachments/assets/a58d535c-6a1e-41c2-97d7-b3b1842e2a3c)

## 🚀 Overview

The **Intelligent Energy Management System (IEMS)** is a smart, ESP32-based solution designed to **manage energy flow** between **solar**, **battery**, and **grid power** in real-time. It prioritizes energy efficiency, system protection, and autonomous decision-making using IoT capabilities and a modern **web dashboard**.

Built in response to **SIH 2024 Problem Statement PS 1572**, IEMS contributes to developing a robust Energy Storage System (ESS) that integrates **renewable sources** and enhances **grid stability**.

---

## 🧠 Key Features

- **Multi-Source Power Control** – Smart switching between Solar, Battery, and Grid
- **Live Monitoring** – Track voltage, current, temperature, and system load
- **Automated Decision Logic** – Dynamic switching based on conditions
- **Safety Systems**  
  - Auto shutdown on high temperature (>80°C)  
  - Overcurrent protection  
  - Battery voltage monitoring  
  - Automatic fan control
- **Web Dashboard (v1.6)**  
  - Real-time charts, analytics, and energy trends  
  - Control buttons for Solar/Battery/Grid/Auto  
  - System Efficiency and Status Indicators
- **Fail-Safe Mode** – Ensures fallback functionality during fault conditions

---

## 🛠️ Dependencies

- `Wire.h` – I2C Communication  
- `OneWire` & `DallasTemperature` – Temp sensors  
- `Adafruit_INA219` – Voltage & Current sensing  
- `ZMPT101B`, `EmonLib` – AC voltage & energy monitoring  
- `ESPAsyncWebServer`, `AsyncTCP` – Web server  
- `ArduinoJson` – Data serialization

---

## 📂 Project Structure
```
├── main.ino          # Main program file
├── config.h          # Configuration and pin definitions
├── webui.h           # Web interface HTML/CSS/JS
├── SensorManager.h   # Sensor data management
├── PowerManager.h    # Power source control
├── SensorInit.h      # Sensor initialization
└── Logger.h          # Logging system
```

---

## 🌐 Demo Dashboard

> To view the new dashboard (v1.6), open `CODE/iEMS-v1.6.html` in your browser.

It includes interactive analytics, real-time values, control buttons, system efficiency meter, and alert system.

---
