# Self-Balancing Robot

A two-wheeled self-balancing robot built from scratch using an ESP32 microcontroller, 
MPU-6050 IMU, and DC motors with hall-effect encoder feedback.

## Goal
Implement a PID control loop that reads IMU angle data and drives motors to maintain 
upright balance in real time.

## Hardware
- ESP32 38-pin CP2102 microcontroller
- MPU-6050 IMU (accelerometer + gyroscope)
- TB6612FNG dual motor driver
- N20 12V 300RPM motors with hall-effect encoders
- 7.4V 2S LiPo battery
- LM2596 buck converter

## Status
- [x] ESP32 flashed and confirmed working
- [ ] IMU data over serial
- [ ] Motor actuation
- [ ] PID implementation
- [ ] Full balancing

## Build Log
**6/26** — ESP32 flashed successfully, onboard LED blinking confirmed
