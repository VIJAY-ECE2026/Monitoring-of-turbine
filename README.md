# Turbine Condition Monitoring System

## Overview
The **Turbine Condition Monitoring System** is designed to detect anomalies in turbine operations using **audio and pressure sensors**. It utilizes **NanoEdge AI** for real-time anomaly detection and is implemented on an **STM32L432KC** microcontroller. This system helps in predictive maintenance, reducing downtime, and ensuring efficient turbine performance.

## Features
- **Real-time condition monitoring** using sound and pressure sensors
- **AI-based anomaly detection** using NanoEdge AI Studio
- **Low-power embedded solution** implemented on STM32L432KC
- **Data acquisition and preprocessing** with STM32CubeIDE
- **Simulation and validation** of AI models with real sensor data

## Components Used
### Hardware:
- **STM32L432KC** (Main microcontroller)
- **Sound sensor** (for acoustic monitoring)
- **Pressure sensor** (for pressure variation detection)
- **Power supply unit**
- **Communication interfaces** (USART, I2C, SPI as needed)

### Software:
- **STM32CubeIDE** (for firmware development)
- **NanoEdge AI Studio** (for training and deploying AI models)
- **Proteus** (for initial simulation and validation)
- **MATLAB/Python** (for additional data analysis and visualization)

## System Architecture
1. **Data Collection:**
   - Sound and pressure sensors collect raw data from the turbine.
   - STM32 reads sensor values periodically.
   
2. **Preprocessing:**
   - Noise filtering and feature extraction from the raw data.
   - Data normalization for AI processing.
   
3. **AI Model Integration:**
   - Anomaly detection model is trained using NanoEdge AI Studio.
   - The model is embedded in STM32 firmware.
   
4. **Real-time Monitoring:**
   - The AI model processes real-time sensor data.
   - Alerts are triggered if anomalies are detected.
   
5. **Data Logging & Communication:**
   - Logs are stored for further analysis.
   - Data is transmitted to a remote system via USART/SPI/I2C if required.

## Installation & Setup
1. **Hardware Setup:**
   - Connect the sensors to the STM32L432KC.
   - Ensure proper power connections and signal integrity.

2. **Software Setup:**
   - Install **STM32CubeIDE** and set up the development environment.
   - Install **NanoEdge AI Studio** and generate an anomaly detection model.
   - Flash the firmware onto the STM32 using a debugger (ST-Link/V2).

3. **Testing & Deployment:**
   - Validate sensor readings and ensure proper data acquisition.
   - Run test cases to verify AI-based anomaly detection.
   - Deploy and monitor performance in real turbine conditions.

## Future Improvements
- Adding **wireless communication (LoRa, BLE, Wi-Fi)** for remote monitoring.
- Enhancing **AI models** with more training data.
- Implementing **cloud storage** for long-term data analysis.
- Developing a **user interface/dashboard** for better visualization.

## References
- STM32 Official Documentation: [https://www.st.com](https://www.st.com)
- NanoEdge AI Studio: [https://www.nanoedgeai.st.com](https://www.nanoedgeai.st.com)
- Embedded AI Applications: [https://www.stmcu.ai](https://www.stmcu.ai)




