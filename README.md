# IoT-Based Health Monitoring System

## Overview

This project focuses on developing an IoT-based health monitoring system using the ESP32 microcontroller and multiple biomedical sensors. The system is designed to acquire physiological parameters, including heart rate, blood oxygen saturation (SpO₂), body temperature, and electrocardiogram (ECG) signals.

The project integrates sensor interfacing and embedded system development to explore real-time physiological data acquisition and monitoring.

## Objectives

- Monitor heart rate and SpO₂ using the MAX30100 pulse oximeter sensor.
- Measure temperature using the LM35 temperature sensor.
- Acquire ECG signals using the AD8232 ECG sensor module.
- Interface multiple sensors with the ESP32 microcontroller.
- Explore real-time health data monitoring using an embedded system.

## Hardware Components

| Component | Function |
|---|---|
| ESP32 | Main microcontroller and sensor interfacing |
| MAX30100 | Heart rate and SpO₂ measurement |
| LM35 | Temperature sensing |
| AD8232 | ECG signal acquisition |
| Jumper wires and breadboard | Circuit connections and prototyping |

## System Architecture

The system follows this general data acquisition flow:

**Biomedical Sensors → ESP32 → Data Processing → Health Parameter Display**

The sensors acquire physiological signals and measurements, which are interfaced with the ESP32 for processing and monitoring.

## Hardware Implementation

### 1. Heart Rate and SpO₂ Monitoring
The MAX30100 uses optical sensing to acquire photoplethysmography (PPG) signals, from which heart rate and estimated oxygen saturation can be calculated.

### 2. Temperature Monitoring
The LM35 generates an analog voltage proportional to temperature. The ESP32 reads this signal through an ADC input and converts it into a temperature measurement.

### 3. ECG Signal Acquisition
The AD8232 conditions the electrical signal acquired through ECG electrodes, providing an output suitable for sampling by the microcontroller's ADC.

### 4. Sensor Integration
The ESP32 serves as the central controller, interfacing with the MAX30100 through I²C and acquiring analog outputs from the LM35 and AD8232.

## Tools and Technologies

- ESP32 microcontroller
- Arduino IDE
- Embedded C/C++
- I²C communication
- ADC-based sensor interfacing
- Biomedical sensors and signal acquisition


