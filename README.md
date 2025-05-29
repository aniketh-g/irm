# Ball Balancing Platform – ETH Zurich (Spring 2025)

This repository contains code developed for the **Introduction to Robotics and Mechatronics** course at ETH Zurich, Spring 2025. The final project involved building a parallel-actuated platform that balances a ball using control algorithms.

This is a glimpse of the final result:

![Ball Balancing Demo](circular_demo.gif)

## Project Goal

To design and control a ball-balancing platform with two modes:
- **Stabilization Mode**: Keeps the ball fixed at a target position.
- **Circular Mode**: Moves the ball in a circular path of a defined radius.

---

## System Setup

- **PixyCam**: Tracks the ball position using computer vision.
- **Platform**: Parallely actuated by three servo motors.
- **Ball**: A ping pong ball moves on the surface.
- **Controller**: An ESP32 Featherboard reads camera input and controls the servos.

---

## Project Workflow

1. **System Modeling**
   Understand how servo angles change the platform’s orientation and how the ball responds to small tilts in the platform.

2. **Inverse Kinematics**
   Compute the servo angles required to achieve a desired platform orientation.

3. **Data Acquisition & Processing**
   Read ball position from the PixyCam, filter the data, apply coordinate transformations, and distortion correction to get the present state of the physical system.

4. **Control Algorithm**
   Use PID control to compute servo commands based on the platform’s current state and target trajectory.

5. **PID Tuning**
   Adjust parameters to ensure smooth and accurate control.

---

## Contributors

Alexander Bilibin

Aniketh Ganesh

Yannick Trommsdorf
