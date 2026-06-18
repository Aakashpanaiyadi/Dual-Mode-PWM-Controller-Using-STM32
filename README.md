# STM32 Motor Control with Local and Remote Operation

## Introduction

This project demonstrates a DC motor control system using an STM32F103 microcontroller. The motor can operate in two modes:

1. **Local Mode** – The STM32 reads an analog input and adjusts the motor speed using PWM.
2. **Remote Mode** – An external controller sends the desired PWM duty cycle through UART, allowing remote speed control.

A switch is used to select between local and remote operation.

## Hardware Used

* STM32F103 Microcontroller
* 9V DC Motor
* N-Channel MOSFET Motor Driver
* 9V Battery
* Mode Selection Switch
* Arduino Nano (External Controller)
* Potentiometer (Analog Speed Input)
* Connecting Wires

## System Overview

In local mode, the STM32 reads the potentiometer value using its ADC and generates a PWM signal to control the motor speed.

In remote mode, the Arduino Nano sends a PWM duty cycle value to the STM32 through UART communication. The STM32 receives this value and updates the PWM output accordingly.

## Communication

* Interface: UART
* Controller: Arduino Nano
* Target Device: STM32F103
* Purpose: Transfer PWM duty cycle values for remote motor control.

## Features

* Dual control modes (Local and Remote)
* ADC-based speed control
* UART-based remote control
* PWM motor speed regulation
* Simple hardware design
* Low-cost implementation

## Applications

* Remote motor control systems
* Robotics projects
* Embedded systems learning
* Industrial control demonstrations
* PWM and UART communication experiments
