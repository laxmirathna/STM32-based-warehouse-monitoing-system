# 🏭 STM32-Based Warehouse Monitoring System

### Real-Time Gas Leakage Detection & Object Monitoring Using STM32

## 📌 Project Overview

The STM32-Based Warehouse Monitoring System is an embedded systems project developed to demonstrate real-time warehouse safety monitoring using an STM32 microcontroller.

The system integrates an MQ Gas Sensor and an Ultrasonic Sensor to monitor environmental conditions and detect nearby objects.

The STM32 processes sensor signals using its ADC and Timer Input Capture peripherals. The processed information is transmitted to a computer through UART communication, where live sensor data can be monitored using PuTTY.

The project demonstrates practical implementation of microcontroller peripherals, sensor interfacing, serial communication, and embedded firmware development.

## 🎯 Project Objectives

- Develop an STM32-based warehouse monitoring prototype.
- Detect gas leakage using an MQ Gas Sensor.
- Detect nearby objects using an Ultrasonic Sensor.
- Implement ADC-based sensor data acquisition.
- Configure Timer Input Capture for distance measurement.
- Establish UART communication between STM32 and PC.
- Display real-time monitoring information through PuTTY.

## ✨ Key Features

- Gas leakage detection using ADC.
- Ultrasonic object detection using Timer Input Capture Direct Mode.
- Configurable gas detection threshold.
- Configurable object detection distance.
- Real-time sensor data transmission through UART.
- PC-based monitoring using PuTTY.
- Embedded firmware development using STM32CubeIDE.

## 🔧 Hardware Components

| Component | Purpose |
|---|---|
| STM32 Microcontroller | Main processing unit |
| MQ Gas Sensor | Gas leakage detection |
| Ultrasonic Sensor | Object detection and distance measurement |
| USB-to-Serial / Debug Interface | Development and communication, as applicable |
| Computer | Monitoring sensor information |

## ⚙️ Working Principle

### 1. Gas Leakage Detection

The MQ Gas Sensor provides an analog output corresponding to the detected gas concentration.

The STM32 reads the analog signal through its ADC peripheral and compares the ADC value with the configured threshold of 900.

When the threshold condition is reached, the system generates a gas detection alert.

### 2. Object Detection

The Ultrasonic Sensor is used to detect nearby objects.

The STM32 uses Timer Input Capture Direct Mode to measure the duration of the ultrasonic echo signal and determine the object distance.

The configured detection range is 10 cm.

### 3. UART Communication

The STM32 transmits sensor readings and monitoring information to a computer through UART communication.

PuTTY is used as the serial terminal to observe the transmitted data in real time.

## 🧠 STM32 Peripheral Implementation

| Peripheral | Application |
|---|---|
| ADC | MQ Gas Sensor data acquisition |
| Timer Input Capture | Ultrasonic echo measurement |
| UART | Serial data transmission to PC |

## 💻 Software and Development Tools

- STM32CubeIDE
- Embedded C
- STM32 Microcontroller Development Environment
- ADC Configuration
- Timer Input Capture
- UART Communication
- PuTTY Serial Terminal

## 📊 Configured Detection Parameters

| Parameter | Configured Value |
|---|---|
| Gas Detection Threshold | 900 ADC |
| Object Detection Range | 10 cm |
| Communication | UART |

## 🧪 Testing and Validation

The system was tested under multiple detection scenarios to verify:

- Gas sensor ADC reading acquisition.
- Gas detection threshold operation.
- Ultrasonic object detection.
- Timer Input Capture operation.
- UART data transmission.
- Real-time monitoring through PuTTY.

The project demonstrated the integration of sensor interfacing and STM32 peripherals for embedded monitoring applications.

## 📁 Project Documentation

This project documentation includes:

- System Architecture Diagram
- Circuit Diagram
- STM32 Pin Configuration
- Hardware Setup and Sensor Interface
- Live Sensor Data on PuTTY
- Test Cases and Results

## 📚 Learning Outcomes

Through this project, I gained practical experience in:

- STM32 Microcontroller Programming
- Embedded C Development
- ADC Configuration and Sensor Interfacing
- Timer Input Capture
- UART Serial Communication
- STM32 Peripheral Configuration
- Hardware and Software Integration
- Testing, Debugging, and Troubleshooting

## 🚀 Future Enhancements

- Add an OLED or LCD display for local monitoring.
- Integrate wireless communication for remote monitoring.
- Introduce data logging for historical analysis.
- Add additional environmental sensors.
- Develop an advanced warehouse monitoring dashboard.

## 🏭 Applications

- Warehouse safety monitoring
- Gas leakage detection
- Industrial safety systems
- Object proximity monitoring
- Embedded monitoring applications

## 👩‍💻 Author

**P. Laxmi Rathna**

Electronics and Communication Engineering Student


---

*Building practical embedded solutions through hardware-software integration.*
