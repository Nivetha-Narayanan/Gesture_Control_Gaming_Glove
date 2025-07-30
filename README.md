# 🎮 Gesture-Controlled Gaming Glove

A wearable glove that enables gesture-based game control by translating hand movements into keyboard inputs using Arduino and Python.

## 📌 Project Summary
This project uses the MPU6050 motion sensor to capture hand gestures, which are processed by an Arduino UNO and sent to a Python script that simulates keypresses. The glove offers an intuitive and immersive gaming experience.

## 🔧 Features
- Gesture recognition using 6-axis IMU (accelerometer + gyroscope)
- Real-time serial communication between Arduino and Python
- Simulates arrow key inputs for games using `pyautogui` and `keyboard`
- Embedded into a glove for natural user interaction
- Budget-friendly and beginner-friendly DIY setup

## ⚙️ System Flow
- **MPU6050**: Detects hand movement and orientation  
- **Arduino UNO**: Reads sensor data via I2C and sends it via Serial  
- **Python Script**:
  - `pyserial`: Receives gesture data
  - `pyautogui`, `keyboard`: Simulates keypresses (e.g., arrow keys)

## 🧪 Results
- Smooth and responsive gesture-to-keyboard mapping
- Effective for simple game control
- Minor drift during fast motion, can be reduced with signal filtering

## 📦 Requirements

### Hardware
- Arduino UNO  
- MPU6050 Sensor Module  
- Glove (as wearable base)  
- USB Cable  
- Jumper Wires

### Software
- Arduino IDE  
- Python 3.x  
- Python Libraries:

```bash
pip install pyserial pyautogui keyboard
