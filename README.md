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

## System Overview (Picture)
![System Picture](images/system_picture.png)

## Software Tools
- **STM32CubeIDE**: For coding and flashing the microcontroller.
- **TeraTerm**: Used for serial communication.

## Circuit Diagram
![Block Diagram](https://github.com/user-attachments/assets/f9578a4e-ba86-4841-9377-0ddc8ef61443)


## How It Works
The irrigation system continuously monitors soil moisture using sensors. Based on moisture levels, the **RTOS** manages the tasks of reading sensor data and controlling water pumps. If a sensor detects a moisture level below the defined threshold (e.g., 50%), the corresponding water pump activates to irrigate that area. The system operates using **mutexes** and **interrupts** to ensure smooth, concurrent task execution.

###Code Explanation
### 1. **Pin Initialization**
In this step, the pins for various components (sensors, pumps, relays) are initialized. This includes configuring **GPIO ports** and defining **input/output** modes for the relevant peripherals.

![Intializing pins](https://github.com/user-attachments/assets/d7f4d16c-a636-4d5f-a33a-4125454cf3f6)



### Priority Code 
Here’s how priority levels are defined for each task in the project:
![Task creation](https://github.com/user-attachments/assets/7f1649e9-1ffe-4a0e-a8e6-f31ded1261eb)


### Soil Function
Here’s The soil function defined in the project:

![Soil Function](https://github.com/user-attachments/assets/6d66f3d7-a15b-4d7f-9864-2e56dafe4c47)




## Bill of Materials
| Item                   | Price (INR) | Quantity | Total Cost (INR) |
|------------------------|-------------|----------|------------------|
| Breadboard              | 93          | 1        | 93               |
| STM32F446RE Nucleo-Board| 1799        | 1        | 1799             |
| IR Sensor               | 26          | 1        | 26               |
| Soil Moisture Sensor    | 50          | 3        | 150              |
| Submersible Motor       | 60          | 3        | 180              |
| Cable                   | 99          | 1        | 99               |
| Jumper Wires            | 2           | 40       | 80               |
| Relays                  | 50          | 3        | 150              |
| Battery                 | 20          | 1        | 20               |
| Pipe                    | 50          | 1        | 50               |
| **Total Cost**          |             |          | **2648 INR**     |


## Future Scope
- **IoT Integration:** Add remote control features through a web or mobile app.
- **Additional Sensors:** Integrate temperature and humidity sensors for better irrigation control.
- **Water Conservation:** Implement water-saving methods like rainwater harvesting.

## Video Demo

https://github.com/user-attachments/assets/fa82dd41-3fac-4f00-9d9b-0970a1e04d73


## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
