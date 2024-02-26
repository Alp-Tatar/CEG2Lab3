# CEG3136 – Lab3: Complex State Machine (C) Alarm Monitoring System

## Overview
This repository contains the completed project for implementing a state machine for an alarm system monitoring application. The project was completed as part of Lab3 in CEG3136.

## Project Structure
- **Source Code:** Contains the source code files for all system components.
- **µVision Project:** The µVision project file containing all project configurations.
- **signal.ini:** Configuration file for simulating external events using signal function.

## System Components
1. **Console Application:** Main function of the program. Initializes the Alarm System and handles user input.
2. **Alarm System Central Control:** Manages the system state machine and low-level system components.
3. **Sensor:** Represents the state of a physical sensor component.
4. **Alarm:** Holds the state of a physical alarm bell component.
5. **User:** Database record of a system user, including name, passcode, and privileges.
6. **Super User:** Extension of the User class with superuser privileges.

## User Interface
- **UI Output:** Displays system logging of events.
- **UI Input:** Accepts user login and system control commands.

## State Machine
- Describes the system's behavior based on current state and external events.
- Transition actions include setting alarms on/off and resetting TickCount.

## SysTick Timer
- Cortex-M processors feature a SysTick timer for periodic interrupt generation.
- Used for monitoring sensor triggers, updating system state, and indicating alarms.

## Interrupt Vector
- EXTI0: Triggered by sensors detecting risk events.
- EXTI1: Triggered by keypad for user login.
- EXTI2: Used to display "beep" message during alarms.

## Simulation
- Emulate sensor events using the signal function set_sensors.
- Compile signal.ini and call signal function during simulation to induce sensor events.

## Completed Tasks
- Implemented the system_update_state() function according to the provided state diagram.
- Tested system behavior to ensure all states and transitions were visited.
- Ended simulation by entering 'q' to display FSM state coverage.

## Report
- Included code snippet of the system_update_state() function.
- Provided simulation log showing all FSM cover points with non-zero coverage value.
- Submitted the source code of the entire project after cleaning all targets.

If you have any questions about the project or need further assistance, feel free to reach out.

