# Smart-Energy-Management-for-Rural-School
Smart Energy Management for rural schools in Ogun state, Nigeria


1. Introduction
This project was developed as part of the Ranger Training on Smart Spaces and Energy Management. The training introduced the concept of using centralized systems such as R1000 and Home Assistant Green to unify and control multiple devices within a smart environment.
Based on this concept, this project implements a simplified and practical version of a smart energy hub designed for rural environments with limited infrastructure.

3. Problem Statement
Schools in rural areas such as Mowe, Ogun State face challenges related to energy access and management. These include:
• Unreliable or limited electricity supply
• Lack of tools to monitor energy consumption
• No centralized system for controlling electrical devices
• Inefficient use of available power sources such as generators or solar systems
These issues lead to energy wastage and reduced operational efficiency.

5. Objective
The objective of this project is to design and implement a system that:
• Monitors energy consumption in real time
• Controls electrical appliances from a central point
• Operates without constant internet connectivity
• Synchronizes data to the cloud when a connection is available

7. System Overview
The system functions as a central energy management hub. It collects data from a smart meter, processes it using a microcontroller, and controls connected devices through relays.
When internet connectivity is available, the system synchronizes data to a cloud database for remote monitoring.

9. System Components
• ESP32 microcontroller (central controller)
• PZEM-004T smart energy meter
• Relay module for device control
• Local storage (EEPROM or SPIFFS)
• Firebase for real-time cloud database

11. System Architecture
The system operates as follows:
• The smart meter measures voltage, current, power, and energy consumption
• The ESP32 processes this data and applies control logic
• Relays are used to switch connected appliances on or off
• Data is stored locally when offline
• When a network is available, data is synchronized to Firebase

13. Key Features
Energy Monitoring
The system measures and tracks:
• Voltage
• Current
• Power
• Energy consumption
Device Control
Electrical appliances such as lights and fans are controlled through relays connected to the microcontroller.
Automation
The system can automatically manage power usage based on defined conditions, such as limiting high consumption.
Offline Operation
The system continues to function without internet connectivity by storing data locally.
Cloud Synchronization
When connectivity is restored, the system updates Firebase in real time, enabling remote monitoring.
Dashboard Interface
A dashboard is used to display energy data and control device states.

15. Implementation
A working prototype was developed and tested. The system successfully demonstrates:
• Real-time energy measurement
• Relay-based control of appliances
• Data logging during offline operation
• Real-time data updates to Firebase when connected

17. Impact
This system provides a practical solution for improving energy management in rural schools by:
• Enabling better visibility into energy usage
• Reducing unnecessary power consumption
• Providing centralized control of devices
• Supporting environments with limited connectivity

19. Next Steps
• Conduct extended testing to validate system reliability
• Deploy the system in a selected school in Mowe, Ogun State
• Collect feedback and improve system performance
• Integrate with broader smart home or smart space systems
• Develop a more advanced custom dashboard
• Enhance cloud features for analytics and remote control
20. Conclusion
This project demonstrates the application of smart space concepts in a real-world rural context. By combining energy monitoring, device control, and offline-first design, it provides a scalable approach to managing energy efficiently in underserved environments.
