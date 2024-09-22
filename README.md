# Smart Irrigation System with STM32F446RE Nucleo-board

## Overview
This project presents a **Smart Irrigation System** built using an **STM32F446RE Nucleo-board** and **Real-Time Operating System (RTOS)** concepts. It automates the irrigation process based on soil moisture levels using sensors and relays to control water pumps. The system is designed to optimize water distribution and ensure efficient resource management through multitasking.

## Problem Statement
Develop a smart irrigation system that efficiently controls water distribution based on real-time soil moisture data. The system should ensure synchronized access to shared hardware resources (pumps and relays) using **mutexes** and **semaphores** and manage tasks like sensor data collection and pump activation through **RTOS**.

## Key Features
- **RTOS Multitasking:** Manages concurrent tasks like sensor reading and pump control.
- **Mutex and Semaphores:** Ensures exclusive access to critical resources (e.g., water pumps) to prevent conflicts.
- **Interrupt Handling:** Gives high priority to sensor data acquisition tasks.
- **Automatic Pump Control:** Based on sensor data, water pumps activate when soil moisture levels drop below a set threshold.
- **Parallel Task Execution:** Allows simultaneous data collection from multiple sensors for real-time monitoring.

## Hardware Components
- **STM32F446RE Nucleo-board**
- **Soil Moisture Sensors** (x3)
- **IR Sensor**
- **Relays** (x3)
- **Submersible Motor** (x3)
- **Button Controls**

## Software Tools
- **STM32CubeIDE**: For coding and flashing the microcontroller.
- **TeraTerm**: Used for serial communication.

## How It Works
The irrigation system continuously monitors soil moisture using sensors. Based on moisture levels, the **RTOS** manages the tasks of reading sensor data and controlling water pumps. If a sensor detects a moisture level below the defined threshold (e.g., 50%), the corresponding water pump activates to irrigate that area. The system operates using **mutexes** and **interrupts** to ensure smooth, concurrent task execution.

## Future Scope
- **IoT Integration:** Add remote control features through a web or mobile app.
- **Additional Sensors:** Integrate temperature and humidity sensors for better irrigation control.
- **Water Conservation:** Implement water-saving methods like rainwater harvesting.

## Video Demo
[Upload a video and provide the link here]

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
