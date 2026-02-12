# Arduino-autonomous-car
Designed and implemented an autonomous mobile robot using Arduino and infrared sensors for real-time navigation. Developed embedded C control logic for obstacle detection, object tracking, and behaviour-based motion control.

# Key Features

Real-time infrared sensor integration
Behaviour-based navigation logic
Closed-loop motor control
Embedded C++ implementation (Arduino IDE)
Optimised response latency

# System Overview
This project integrates infrared sensor feedback with motor control to enable autonomous navigation and reactive movement.
The system:
Continuously reads IR sensor input
Detects obstacles or target objects
Executes behaviour-based motion decisions
Controls DC motors via motor driver
Adjusts movement in real time

# Navigation Logic

The navigation algorithm implements behaviour-based decision control:
If obstacle detected → adjust steering
If path clear → move forward
If target detected → track object
If no input → default safe motion state
Sensor data is processed continuously and translated into motor commands for responsive movement.

# Control Strategy
Real-time sensor polling
Conditional behaviour logic
Direct motor speed control
Latency optimisation for improved response time

# Hardware
Arduino Uno
Infrared sensors
DC motors
Motor driver module
Chassis platform
External power supply
