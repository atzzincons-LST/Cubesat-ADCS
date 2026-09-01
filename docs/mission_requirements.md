# Mission Requirements

## 1. Mission Overview

The objective of this project is to develop and validate a simulated Attitude Determination and Control System (ADCS) for a 3U CubeSat operating in Low Earth Orbit.

The spacecraft is assumed to perform an Earth-observation mission requiring three-axis attitude stabilization and controlled pointing.

## 2. Preliminary Mission Parameters

| Parameter | Value |
|---|---|
| Spacecraft configuration | 3U CubeSat |
| Orbit altitude | 500 km |
| Orbit type | Circular LEO |
| Attitude architecture | 3-axis stabilized |
| Primary actuators | Reaction wheels |
| Secondary actuators | Magnetorquers |
| Sensors | Gyroscope, magnetometer, sun sensor |
| Attitude representation | Quaternion |

## 3. Preliminary ADCS Requirements

### 3.1 Pointing Accuracy

The system shall target an attitude pointing error of less than:

**1 degree**

### 3.2 Angular Rate

The system shall target an angular-rate error of less than:

**0.1 deg/s**

### 3.3 Stabilization

The spacecraft shall autonomously reduce an initial attitude error and converge toward the commanded attitude.

### 3.4 Simulation

The ADCS shall be evaluated using a nonlinear spacecraft rotational dynamics model.

### 3.5 Robustness

The system shall be evaluated under:

- Sensor noise
- Sensor bias
- Initial attitude uncertainty
- Initial angular-rate uncertainty
- Spacecraft inertia uncertainty
- Actuator limitations

## 4. Verification

The system will be evaluated through numerical simulation and Monte Carlo analysis.

Performance metrics will include:

- Pointing error
- Angular-rate error
- Settling time
- Overshoot
- Control effort
- Estimator error
- Actuator saturation

## 5. Requirement Status

These requirements are preliminary and will be refined as the spacecraft model and mission concept develop.
