# Arduino-autonomous-car
Designed and implemented a state-machine-driven autonomous robot using encoder-based position control and infrared distance tracking. Integrated closed-loop PI controllers for both motion profiling and real-time distance regulation.

# Key Features

Quadrature encoder feedback with interrupt handling
Position-based PI motor control
IR distance-based PI tracking control
Finite state machine for sequential task execution
Servo actuation with timed sequencing
LED-based status indication
10 ms real-time control loop

# System Overview
This project combines position control, distance tracking, and event-driven sequencing into a structured embedded control architecture.
The robot:
Waits for a button press
Lowers and raises a servo-actuated mechanism
Executes a predefined motion sequence:
Forward 15 cm
Backward 30 cm
Forward 30 cm
Backward 15 cm
Switches to IR-based closed-loop distance tracking for 20 seconds
Stops and flashes LEDs before reset

# Control Strategy
Position Control Mode

Target distance converted to encoder counts

PI controller drives motor to reference position

Soft scaling near target to reduce overshoot

Minimum PWM enforcement to prevent stalling

IR Distance Tracking Mode

Averaged IR sensor sampling

Nonlinear voltage-to-distance conversion

PI control to maintain ~30 cm distance

Automatic switching between control modes

# Hardware
Arduino

DC motor with quadrature encoder

Motor driver

Infrared distance sensor

Servo motor

Push button

Status LED
