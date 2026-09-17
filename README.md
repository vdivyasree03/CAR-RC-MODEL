# RC Car – Remote Control & Obstacle Avoidance

An embedded **Remote-Controlled and Obstacle-Avoidance Car** built using an **STM32F4 microcontroller** and an **ESP32 Bluetooth module**.

## 🚀 Overview

This project is a small embedded robotics system that combines Bluetooth communication, motor control, sensor interfacing, and obstacle detection.

The **ESP32** is used as the Bluetooth communication interface, while the **STM32F4** handles the main control logic, sensor input, and motor control.

## ✨ Features

- Bluetooth-controlled RC car
- Obstacle avoidance
- STM32F4-based control system
- ESP32 Bluetooth communication
- DC motor control
- Sensor interfacing
- Real-time control
- Embedded firmware
- Robotics application

## 🛠️ Technologies Used

- STM32F4
- STM32F401
- ESP32
- Embedded C / C++
- Bluetooth
- Motor Control
- Sensors
- Embedded Systems
- Microcontrollers

## ⚙️ System Architecture

```text
          Bluetooth Controller
                   │
                   ▼
                ESP32
          Bluetooth Interface
                   │
                   ▼
                STM32F4
            Main Control Logic
              │           │
              │           │
              ▼           ▼
       Obstacle Sensor  Motor Driver
              │           │
              │           ▼
              │        DC Motors
              │           │
              └──────────► │
                          ▼
                       RC Car
```

## 🎮 Remote Control Mode

The car can receive movement commands through Bluetooth.

```text
Forward
Backward
Left
Right
Stop
```

The ESP32 receives the Bluetooth command and communicates the required control information to the STM32F4.

The STM32 then controls the motors according to the received command.

## 🚧 Obstacle Avoidance Mode

The car uses an obstacle/distance sensor to detect objects in its path.

When an obstacle is detected, the controller can stop the vehicle or change its direction according to the programmed logic.

## 🔄 Control Flow

```text
              Start
                │
                ▼
      Initialize STM32
                │
                ▼
      Initialize ESP32
          Bluetooth
                │
                ▼
       Read Bluetooth
          Command
                │
        ┌───────┴────────┐
        │                │
        ▼                ▼
 Movement Command   Obstacle Detected
        │                │
        ▼                ▼
  Control Motors    Stop / Change
                     Direction
        │                │
        └───────┬────────┘
                ▼
              Repeat
```

## 🔧 Hardware Requirements

- STM32F4 development board
- STM32F401 microcontroller/board
- ESP32 development board/module
- DC motors
- Motor driver
- Obstacle/distance sensor
- RC car chassis
- Battery/power supply
- Jumper wires
- Breadboard

## 💻 Software Requirements

- STM32CubeIDE or compatible STM32 development environment
- ESP32 development environment
- Embedded C/C++
- STM32 HAL/peripheral libraries

## 🏗️ Setup

1. Connect the STM32F4 to the motor driver.
2. Connect the obstacle sensor to the STM32.
3. Connect the ESP32 as the Bluetooth communication interface.
4. Upload the STM32 firmware.
5. Upload/configure the ESP32 Bluetooth firmware.
6. Power the complete system.
7. Establish a Bluetooth connection.
8. Send movement commands and test the car.
9. Test obstacle detection and avoidance.

## 📚 What I Learned

- STM32F4 microcontroller programming
- STM32 peripheral configuration
- ESP32 Bluetooth communication
- Motor-driver interfacing
- Sensor interfacing
- Embedded control logic
- Real-time embedded programming
- Hardware and firmware debugging
- Embedded robotics development

## 🔮 Future Improvements

- Add autonomous navigation
- Add PWM-based speed control
- Develop a mobile application
- Add live sensor data
- Improve obstacle-avoidance logic
- Add battery-level monitoring
- Add multiple driving modes
- Add wireless telemetry

## 📄 License

This project is created for educational and personal development purposes.
