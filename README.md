# BTS and Arduino Shield for Motor and Actuator Control

## Overview

This project is a custom-designed shield for Arduino, intended for controlling motors and actuators using the **BTS Linear Actuator Driver** and **A4988 Stepper Motor Driver**. It provides an interface to control different types of motors, including DC motors and stepper motors, and includes features to adjust sensitivity and control modes. This shield is well-suited for robotics, automation, and projects that require precise control of linear and rotational motion.

## Features

- **BTS Linear Actuator Driver**:
  - Capable of controlling linear actuators for various automation applications.
  - Supports PWM control for precise actuator positioning.
  - Provides GND, LPWM, RPWM, and VCC pins for easy connectivity.

- **DC Motor Driver**:
  - Designed to handle DC motors with configurable settings.
  - Control pins include GND, PWM, and VCC to ensure flexible power options.

- **A4988 Stepper Motor Driver**:
  - Allows precise step and direction control of stepper motors.
  - Supports microstepping for smoother motion control.
  - Includes pins for STEP and DIR signals, plus power (VCC and GND).

- **RC Mode Configuration**:
  - Includes selectable configurations for 1ms and 2ms pulse width signals.
  - Adjustable sensitivity settings for controlling motor or actuator response.
  - LED indicators to show signal status and activity.

- **Analog and Potentiometer Mode**:
  - Potentiometer inputs allow for manual control of the motor or actuator's position.
  - Voltage input mode supports 0-5V control, suitable for analog signal control systems.

## Control Settings

The shield offers several control options, configured via jumpers and potentiometers:

1. **RC Mode (1ms and 2ms Pulse Width)**:
   - Jumper settings enable selection between 1ms and 2ms pulse widths, commonly used in RC servo control applications.
   - Supports independent power supply to prevent interference with Arduino’s power supply.
   - Simple wiring with three connections: RC (signal), GND, and VCC (optional, only if needed).

2. **Voltage and Potentiometer Input Mode**:
   - This mode allows controlling the motor or actuator using analog voltage (0-5V) or a potentiometer.
   - Adjustable potentiometer inputs (10k, 50k, 100k) for manual tuning.
   - Ideal for applications where precise, hands-on control is required.

3. **Adjustable Sensitivity**:
   - Two potentiometers for adjusting the sensitivity range and rotation angle of the actuator or motor.
   - These allow fine-tuning to fit specific use cases, making the shield versatile for various control applications.

## Specifications

- **Dimensions**: 117.13 mm x 68.63 mm (fits standard Arduino form factor)
- **Input Voltage**: Supports 5V input for digital controls, 0-5V analog input for potentiometer control.
- **Compatibility**: Compatible with Arduino and other microcontroller boards with similar pin layouts.

## Setup and Usage

1. **Power Supply**:
   - Connect the DC power supply to the `DC POWER INPUT` terminals.
   - Ensure correct polarity when wiring, as reversing power input may damage the shield.

2. **Jumper Configuration**:
   - Use the jumpers to switch between different modes (RC Mode, Potentiometer Mode).
   - Set the desired pulse width or analog control mode as per your application.

3. **Connections**:
   - Connect your actuator or motor to the appropriate terminals (e.g., BTS Linear Actuator, DC Motor, Stepper Motor).
   - Use the Arduino’s digital or analog pins to control the actuator or motor based on the selected mode.

4. **Tuning and Adjustments**:
   - Use the potentiometers on the board to adjust the sensitivity and rotation angle range for optimal control response.
   - Refer to the LED indicators for feedback on control signals and operational status.

## Warnings

- **Power Input Polarity**: Ensure correct polarity when connecting the power supply. Incorrect wiring can cause permanent damage to the shield and connected components.
- **Independent Power for Servos**: When using RC Mode, provide an independent power supply for servos if necessary, as indicated in the documentation.

## Applications

This shield is suitable for applications requiring precise and configurable motor or actuator control, including:

- Robotics and automation systems
- Remote-controlled vehicles and drones
- Linear positioning systems
- Custom servo control setups
