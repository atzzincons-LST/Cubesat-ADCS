# 3U CubeSat Attitude Determination and Control System

A spacecraft Guidance, Navigation and Control (GNC) project focused on the design, simulation, estimation, and control of a 3U CubeSat attitude control system.

## Project Overview

This project develops a complete Attitude Determination and Control System (ADCS) for a simulated 3U CubeSat operating in Low Earth Orbit (LEO).

The project will progressively implement:

- Spacecraft rotational dynamics
- Quaternion-based attitude representation
- Attitude kinematics
- Reaction wheel actuation
- Magnetorquer actuation
- Gyroscope modeling
- Magnetometer modeling
- Sun sensor modeling
- Attitude determination
- Extended Kalman Filter (EKF)
- PID attitude control
- Linear Quadratic Regulator (LQR)
- Environmental disturbances
- Sensor noise and bias
- Monte Carlo performance analysis
- Hardware-in-the-loop implementation

## Mission Concept

| Parameter | Initial Value |
|---|---|
| Spacecraft | 3U CubeSat |
| Mission | Earth observation |
| Orbit | 500 km LEO |
| Attitude Control | 3-axis stabilized |
| Primary Control | Reaction wheels |
| Momentum Management | Magnetorquers |
| Attitude Representation | Quaternions |
| Estimator | EKF |
| Controllers | PID / LQR |

*The mission parameters are preliminary and will be refined as the project develops.*

## System Architecture

The ADCS architecture will consist of:

```text
Sensors
   │
   ▼
Attitude Determination
   │
   ▼
State Estimation
   │
   ▼
Controller
   │
   ▼
Actuators
   │
   ▼
Spacecraft Dynamics
   │
   └──────────────► Sensors
