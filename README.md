<div align="center">

# 🌊 AQUA SENSE

### Smart River Water Quality Monitoring System

**Monitor · Analyze · Protect**

An IoT-based solution for monitoring river water quality through smart sensors and real-time data visualization.

<br>

![IoT](https://img.shields.io/badge/IoT-Smart_Monitoring-2E8B57?style=for-the-badge)
![Arduino](https://img.shields.io/badge/Arduino-Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![ESP8266](https://img.shields.io/badge/ESP8266-Wireless-orange?style=for-the-badge)
![Python](https://img.shields.io/badge/Python-Flask-3776AB?style=for-the-badge&logo=python&logoColor=white)

</div>

---

## 🌍 Project Overview

Aqua Sense is an **IoT-based river water quality monitoring system** designed to measure important water quality parameters and visualize sensor readings through a web dashboard.

The system combines hardware sensors, wireless communication, and web technologies to support environmental monitoring and river conservation.

---

## 🔬 What We Monitor

<div align="center">

| 🌡️ Temperature | 🌫️ Turbidity | 💧 TDS |
|:---:|:---:|:---:|
| DS18B20 | SEN0189 | TDS Sensor V1.0 |
| Water temperature | Water cloudiness | Dissolved solids estimation |

</div>

---

## ⚙️ System Architecture

<div align="center">

```mermaid
flowchart TD
    A["🌊 River Water"] --> B["🔬 Sensors"]

    B --> C["Arduino Uno"]

    C --> D["ESP8266"]

    D --> E["📡 Wi-Fi"]

    E --> F["🐍 Flask API"]

    F --> G["📊 Web Dashboard"]

    G --> H["🌱 Environmental Insights"]

    style A fill:#e0f2fe,stroke:#0284c7,color:#0c4a6e
    style B fill:#dcfce7,stroke:#16a34a,color:#14532d
    style C fill:#fef3c7,stroke:#d97706,color:#78350f
    style D fill:#fef3c7,stroke:#d97706,color:#78350f
    style F fill:#f3e8ff,stroke:#9333ea,color:#581c87
    style G fill:#e0f2fe,stroke:#0284c7,color:#0c4a6e
```

</div>

### 🔄 Data Flow

<div align="center">

**Sensors → Arduino → ESP8266 → Wi-Fi → Flask Backend → Dashboard**

</div>

---

## 🧠 Technology Stack

<div align="center">

| Layer | Technology |
|:---:|:---|
| 🔬 Sensing | DS18B20 · SEN0189 · TDS Sensor |
| ⚡ Processing | Arduino Uno |
| 📡 Communication | ESP8266 · Wi-Fi |
| 🖥️ Backend | Python · Flask |
| 📊 Frontend | HTML · CSS · JavaScript |

</div>

---

## ✨ Key Features

<div align="center">

| 🌡️ | 💧 | 📡 |
|:---:|:---:|:---:|
| Temperature Monitoring | TDS Measurement | Wireless Communication |

| 🌫️ | 📈 | 🌍 |
|:---:|:---:|:---:|
| Turbidity Monitoring | Data Visualization | Environmental Monitoring |

</div>

- Real-time sensor data collection
- Wireless transmission of measurements
- Web-based water quality dashboard
- Visual representation of water quality parameters
- Backend API for sensor communication
- Designed for river monitoring and environmental awareness

---

## 🔌 Hardware Components

<div align="center">

| Component | Purpose |
|:---|:---|
| Arduino Uno | Sensor data acquisition |
| ESP8266 | Wi-Fi communication |
| DS18B20 | Temperature measurement |
| SEN0189 | Turbidity measurement |
| TDS Sensor V1.0 | TDS estimation |
| Voltage Regulator | Power regulation |

</div>

---

## 📡 Backend API

The Flask backend supports sensor communication through the following endpoints:

<div align="center">

| Method | Endpoint | Function |
|:---:|:---:|:---|
| `GET` | `/data` | Current sensor readings |
| `GET` | `/history` | Historical measurements |
| `POST` | `/data` | Submit sensor data |

</div>

---

## 🚀 How It Works

<div align="center">

```mermaid
sequenceDiagram
    participant S as Sensors
    participant A as Arduino Uno
    participant E as ESP8266
    participant B as Flask Backend
    participant D as Dashboard

    S->>A: Collect measurements
    A->>E: Send sensor values
    E->>B: Transmit through Wi-Fi
    B->>B: Process incoming data
    B->>D: Provide readings
    D->>D: Visualize water quality
```

</div>

---

## 🌱 Applications

<div align="center">

| 🌊 | 🧪 | 🎓 |
|:---:|:---:|:---:|
| River Monitoring | Environmental Research | Educational Projects |

| 🌍 | 📊 | 💧 |
|:---:|:---:|:---:|
| Water Conservation | Data Analysis | Water Quality Awareness |

</div>

---

## 🔮 Future Scope

<div align="center">

```mermaid
mindmap
  root((Aqua Sense))
    Smart Monitoring
      Sensor Integration
      Continuous Data
    Intelligent Analysis
      AI Prediction
      Anomaly Detection
    Advanced Visualization
      Geographic Mapping
      Historical Trends
    Environmental Impact
      River Conservation
      Pollution Awareness
```

</div>

- 🗺️ Geographic water quality visualization
- 🤖 AI-based water quality trend analysis
- 📍 Pollution source mapping
- ☁️ Cloud-based data storage
- 🚨 Water quality anomaly alerts
- 📱 Mobile-friendly monitoring interface

---

## ⚠️ Important Note

Aqua Sense is an evolving IoT prototype for environmental monitoring.

The measured parameters alone cannot establish whether water is safe for drinking or identify specific pollutants.

Reliable interpretation requires proper calibration, validation, and laboratory testing where necessary.

---

<div align="center">

## 🌊 Turning Water Data into Environmental Awareness

### Built with 💚 for Cleaner Rivers

**Aqua Sense**

</div>
