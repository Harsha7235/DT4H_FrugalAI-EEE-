# 🏥 DT4H – Digital Twin for Healthcare
### An IoT-Enabled Cyber-Physical System for Intelligent Health Monitoring

**DT4H (Digital Twin for Healthcare)** is a Cyber-Physical System (CPS) project that combines embedded hardware, IoT communication, digital twin modelling, cloud technologies, and intelligent health-risk monitoring.

The project aims to create a virtual representation of a person's physiological condition by collecting health-related parameters, processing them, and synchronizing the information with a digital monitoring environment.

It integrates hardware-level monitoring with MATLAB Simulink-based modelling and a cloud-connected software architecture.

---

## 🎯 Project Objectives

- Develop an IoT-based health-monitoring prototype.
- Simulate and monitor physiological parameters.
- Establish communication between embedded hardware and a cloud-connected server.
- Develop a digital twin representation of health parameters.
- Identify abnormal readings through threshold-based risk evaluation.
- Generate visual and audible alerts for warning and danger conditions.
- Explore AI-assisted anomaly detection and predictive monitoring.
- Incorporate blockchain-inspired logging for data integrity and traceability.

---

## ⚙️ System Architecture

DT4H follows a multi-layer Cyber-Physical System architecture.

### 1. Physical Hardware Layer
The hardware layer represents the physical monitoring system.

Components include:
- Arduino Mega
- ESP32 Development Board
- LM35 Temperature Sensor / simulated temperature input
- Heart Rate and SpO₂ sensor interfaces
- Potentiometers for simulated physiological inputs
- 16×2 I2C LCD Display
- Green, Yellow and Red LEDs
- Buzzer

### 2. Data Acquisition Layer
The microcontroller acquires physiological parameter values from sensors or simulated inputs.

The Arduino processes the readings and evaluates their status using predefined thresholds.

### 3. Edge Processing and Communication Layer
The Arduino Mega communicates with the ESP32 through serial communication.

The ESP32 provides Wi-Fi connectivity and transmits structured health data to the Node.js server using HTTP requests.

### 4. Digital Twin and Cloud Layer
The Node.js server receives and processes incoming health information.

The cloud-connected application provides a digital representation of the monitored parameters, allowing users to view current readings and system status.

### 5. Monitoring and Alert Layer
The system evaluates health parameters and identifies normal, warning, and risk conditions.

- Green LED – Normal condition
- Yellow LED – Warning condition
- Red LED – Critical/risk condition
- Buzzer – Audible warning indication
- LCD – Displays parameter values and health status

### 6. Simulation and Validation Layer
MATLAB Simulink is used to develop and simulate the cyber-physical architecture.

The model includes synthetic data generation, preprocessing, feature extraction, digital twin modelling, predictive decision logic, anomaly detection, and dashboard outputs.

### 7. Security and Audit Layer
A lightweight blockchain-inspired ledger is incorporated into the architecture to explore data integrity, event traceability, and secure health-data logging.

---

## 🔄 Working Process

```text
Physiological Parameters
          |
          v
Sensor / Simulated Data Acquisition
          |
          v
Arduino Mega Processing
          |
          v
Threshold Evaluation
          |
          +------> LCD Display
          |
          +------> LED Indicators
          |
          +------> Buzzer Alerts
          |
          v
ESP32 Wireless Communication
          |
          v
Node.js Server / API
          |
          v
Digital Twin and Data Processing
          |
          +------> Health Monitoring Dashboard
          |
          +------> Event Logging
          |
          +------> Anomaly Analysis
          |
          v
Cloud-Based Monitoring
```

---

## 🧠 MATLAB Simulink Model

The Simulink implementation models the DT4H cyber-physical workflow.

Major subsystems include:

1. **Synthetic Data Generation** – Generates simulated physiological input signals.
2. **Preprocessing** – Filters and prepares incoming data.
3. **Feature Extraction** – Extracts relevant health parameters.
4. **Digital Twin Model** – Represents physiological behaviour using state-space modelling.
5. **Predictive Model and Decision System** – Evaluates health conditions using MATLAB Function blocks, moving averages, comparisons, and fuzzy logic.
6. **Anomaly Detection** – Identifies abnormal parameter behaviour.
7. **Dashboard** – Provides visual monitoring of system outputs.

The model helps evaluate the system's behaviour under different input conditions before and alongside hardware implementation.

---

## 🛠️ Technologies Used

| Category | Technologies |
|---|---|
| Embedded Systems | Arduino Mega, ESP32 |
| Hardware Programming | Arduino IDE, Embedded C/C++ |
| Simulation | MATLAB, Simulink |
| Backend | Node.js, Express.js |
| Communication | UART Serial, Wi-Fi, HTTP, REST API |
| Frontend | Web-based monitoring dashboard |
| Cloud Deployment | Render |
| Notifications | Twilio SMS integration |
| Security | Blockchain-inspired ledger, hash-based integrity concepts |
| Data Processing | Signal Processing, Moving Average, Threshold Evaluation |
| Intelligent Analysis | Anomaly Detection, Predictive Analytics, Fuzzy Logic |

---

## 📊 Health Parameter Monitoring

The system focuses on three primary physiological parameters:

| Parameter | Description |
|---|---|
| Heart Rate (HR) | Monitors heart-rate-related input values |
| SpO₂ | Monitors simulated or sensor-derived oxygen saturation values |
| Temperature | Monitors body-temperature-related input values |

The hardware prototype supports simulated input testing through potentiometers, allowing different operating conditions to be evaluated.

---

## 🔐 Security Concepts

DT4H also explores security within connected healthcare systems.

The security-oriented design includes:

- Blockchain-inspired event logging.
- Timestamped health-data records.
- Hash-based integrity verification concepts.
- Monitoring of abnormal data patterns.
- Exploration of intrusion and anomaly detection.

The ledger implementation should be understood as a lightweight prototype rather than a production blockchain network.

---

## 🚀 Future Enhancements

- Integration of calibrated biomedical sensors.
- Advanced machine-learning-based health anomaly detection.
- Improved predictive analytics.
- Persistent blockchain-based event storage.
- Enhanced cloud database integration.
- More advanced real-time dashboard visualizations.
- Improved authentication and access control.
- Extended mobile monitoring capabilities.

---

## ⚠️ Disclaimer

DT4H is an academic engineering prototype developed for educational, simulation, and research purposes.

It is not a certified medical device and must not be used as a substitute for professional medical diagnosis, treatment, or emergency monitoring.

Some physiological inputs may be simulated for testing and validation.

---

## 👨‍💻 Project Information

**Project:** DT4H – Digital Twin for Healthcare  
**Domain:** Cyber-Physical Systems, IoT, Digital Twin Technology, Healthcare Technology  
**Institution:** Amrita Vishwa Vidyapeetham, Coimbatore  
**Developer:** Harsha Vardhan Reddy

---

## ⭐ Acknowledgement

This project represents an exploration of how embedded systems, IoT, cloud computing, simulation, and intelligent data processing can be integrated to develop next-generation healthcare monitoring systems.

⭐ If you find this project interesting, consider starring the repository!
