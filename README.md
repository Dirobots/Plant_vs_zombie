# Plant vs Zombie – Automated Basilic Growing System

## Overview

**Plant vs Zombie** is a project focused on optimizing the growth of a **basilic (basil) plant** through a set of automated systems. Rather than relying on manual care, the project leverages sensors, actuators, and control algorithms to create the ideal growing environment for the plant at all times.

## Features

### 🌱 Auto Watering
An automated watering system monitors soil moisture levels and delivers the precise amount of water the plant needs. This prevents both under-watering and over-watering, two of the most common causes of poor plant health.

### 💧 Humidity Detection
Humidity sensors continuously measure the ambient relative humidity around the plant. The readings are used to trigger ventilation or misting systems to keep humidity within the optimal range for basilic growth.

### 💡 Smart Lighting
Automated lighting adjusts the intensity and duration of light exposure based on the plant's current growth stage and the ambient light level. This ensures the basilic receives sufficient photosynthetically active radiation (PAR) throughout the day, even in low-light environments.

### ⚙️ PID Controllers
Each automation subsystem is governed by a **PID (Proportional–Integral–Derivative) controller**, which continuously calculates the error between a desired setpoint and the measured value, then applies a correction to minimize that error. This closed-loop control strategy ensures:

- **Stable, precise regulation** of water, humidity, and light levels.
- **Fast response** to environmental disturbances.
- **Minimal overshoot**, avoiding conditions that could harm the plant.

## How It Works

```
Sensor Reading  →  PID Controller  →  Actuator Command
     ↑                                        |
     └────────────── Feedback Loop ───────────┘
```

1. Sensors (moisture, humidity, light) continuously sample the plant's environment.
2. Each PID controller compares the sensor reading against a configured setpoint.
3. The controller outputs a correction signal to the relevant actuator (pump, fan/mister, grow light).
4. The cycle repeats, keeping all parameters within the optimal range for basilic growth.

## Goals

- Maximize basilic yield and quality through consistent, data-driven care.
- Reduce manual intervention by automating routine plant maintenance tasks.
- Provide a reusable, modular automation platform that can be adapted for other plant species.

