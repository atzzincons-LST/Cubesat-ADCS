# ADCS System Architecture

## 1. Overview

The Attitude Determination and Control System consists of sensors, an attitude determination and estimation subsystem, a control subsystem, actuators, and the spacecraft rotational dynamics.

## 2. Functional Architecture

```text
                  Commanded Attitude
                         │
                         ▼
                 ┌───────────────┐
                 │   Guidance    │
                 └───────┬───────┘
                         │
                         ▼
                 ┌───────────────┐
                 │   Estimator   │
                 │     EKF       │
                 └───────┬───────┘
                         │
                  Estimated State
                         │
                         ▼
                 ┌───────────────┐
                 │   Controller  │
                 │   PID / LQR   │
                 └───────┬───────┘
                         │
                    Control Torque
                         │
                         ▼
                 ┌───────────────┐
                 │   Actuators   │
                 │ Reaction Wheel│
                 │ Magnetorquer  │
                 └───────┬───────┘
                         │
                         ▼
                 ┌───────────────┐
                 │  Spacecraft   │
                 │    Dynamics   │
                 └───────┬───────┘
                         │
                         ▼
                     Attitude
                         │
             ┌───────────┴───────────┐
             │                       │
             ▼                       ▼
          Gyroscope             Magnetometer
             │                       │
             └───────────┬───────────┘
                         │
                         ▼
                     Estimator
