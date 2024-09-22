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

## Block Diagram
![Block Diagram](images/block_diagram.png)

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

## How It Works
The irrigation system continuously monitors soil moisture using sensors. Based on moisture levels, the **RTOS** manages the tasks of reading sensor data and controlling water pumps. If a sensor detects a moisture level below the defined threshold (e.g., 50%), the corresponding water pump activates to irrigate that area. The system operates using **mutexes** and **interrupts** to ensure smooth, concurrent task execution.

## Hardware Connections
![Hardware Setup](images/hardware_setup.png)

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

## Circuit Diagram
![Circuit Diagram](# Smart Irrigation System with STM32F446RE Nucleo-board

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

## Block Diagram
![Block Diagram](images/block_diagram.png)

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

## How It Works
The irrigation system continuously monitors soil moisture using sensors. Based on moisture levels, the **RTOS** manages the tasks of reading sensor data and controlling water pumps. If a sensor detects a moisture level below the defined threshold (e.g., 50%), the corresponding water pump activates to irrigate that area. The system operates using **mutexes** and **interrupts** to ensure smooth, concurrent task execution.

## Hardware Connections
![Hardware Setup](images/hardware_setup.png)

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

## Circuit Diagram
![Circuit Diagram](images/circuit_diagram.png)

## Future Scope
- **IoT Integration:** Add remote control features through a web or mobile app.
- **Additional Sensors:** Integrate temperature and humidity sensors for better irrigation control.
- **Water Conservation:** Implement water-saving methods like rainwater harvesting.

## Video Demo
[Upload a video and provide the link here]

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
)

## Future Scope
- **IoT Integration:** Add remote control features through a web or mobile app.
- **Additional Sensors:** Integrate temperature and humidity sensors for better irrigation control.
- **Water Conservation:** Implement water-saving methods like rainwater harvesting.

## Video Demo
[Upload a video and provide the link here]

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
