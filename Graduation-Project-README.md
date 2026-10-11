# Autonomous Medicine-Delivery Robot for Clinics

Graduation project, HCMC University of Technology and Education, 2023. Team of two.

A small mobile robot that carries medicine to rooms in a clinic. Route planning uses a Deep Q-Network (DQN) trained on a 2D simulation map of the clinic. The robot runs on an Arduino Mega with FreeRTOS.

Portfolio page with photos, simulation map, PCB and schematic: https://vovinhtruong.github.io/#robot

## My part

- Designed and implemented the DQN route planner and the 2D simulation map used to train it
- Simulated the circuit in Proteus
- Programmed the Arduino Mega with FreeRTOS and the sensor modules

The PCB layout was drawn by my teammate.

## Hardware

- Arduino Mega 2560
- L298N motor driver
- LM2596 power supply
- VL53L0X laser distance sensor
- HC-05 Bluetooth module
- 20x4 LCD

## Files

| File | Content |
|---|---|
| `Autonomous_Controller.py` | DQN route planner (Keras), runs on a PC and sends moves to the robot over HC-05 Bluetooth |
| `Autonomous_Robot.ino` | Arduino firmware (FreeRTOS) |
| `model(...).h5`, `model(...).json` | Trained DQN models (Keras weights and architecture) |
