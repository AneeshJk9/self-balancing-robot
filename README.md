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
- [x] IMU data over serial
- [ ] Motor actuation
- [ ] PID implementation
- [ ] Full balancing

## Build Log
**6/26** — ESP32 flashed successfully, onboard LED blinking confirmed
**6/29/2026** — Got live accelerometer/gyro data streaming from the MPU-6050 over I2C. Hit a watchdog-reset bug caused by a loose jumper wire; diagnosed it using an I2C scanner sketch before going back to the main MPU6050_raw sketch. Attached photos of breadboard wiring and Serial Monitor output below.
<img width="1179" height="1439" alt="image" src="https://github.com/user-attachments/assets/d0f07bf4-84ed-4e19-8976-637f02a3a800" />
<img width="1568" height="317" alt="image" src="https://github.com/user-attachments/assets/ea790536-38c5-4ec5-8ace-79cd40f02f36" />


