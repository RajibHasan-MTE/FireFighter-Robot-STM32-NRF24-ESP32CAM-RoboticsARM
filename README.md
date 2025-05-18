# 🚒 FireFighter Robot with STM32, NRF24L01, ESP32-CAM

This is an open-source firefighting robot system that combines embedded systems, wireless communication, IoT, and robotics. The robot is capable of detecting fire, gas leaks, and hazardous environments while sending real-time video feedback. It also includes a 5-DOF robotic arm for pick-and-place tasks and a custom-built wireless controller.
<p align="center">
  <img src="DOCS/image/robot-pic-1.jpg" alt="Pinout" width="800" height="300">
</p>
---

## 📦 Project Overview

### 🤖 Main Robot Features
- **MCU**: STM32 (Main controller)
- **Wireless Video**: ESP32-CAM for real-time video streaming
- **Wireless Communication**: NRF24L01 module
- **Sensors**:
  - Flame Sensor (fire detection)
  - Gas Sensor (MQ-series)
  - Oxygen Sensor
- **Actuators**:
  - 5 Servo Motors (Robotic Arm)
  - High-speed Fan (Fire extinguishing)
  - 800 RPM Gear Motor with Wheels (Locomotion)
- **Communication Module**: GSM for emergency alerts
- **Water Sprayer**: For extinguishing fire

### 🎮 Remote Controller Features
- **MCU**: STM32
- **Wireless Communication**: NRF24L01
- **Input Devices**:
  - 2-Axis Joystick (For movement)
  - 5 × 10k Potentiometers (For robotic arm control)
  - Dedicated switches (Mode/Arm/Light/Fire)
- **Custom PCB Design**: Designed using Altium/EasyEDA (depending on your tools)

---

## 🧠 System Architecture

- **Data Communication**: Robot ↔ Remote via NRF24L01
- **Live Video Feed**: ESP32-CAM over WiFi
- **Emergency Alert**: SMS/Call via GSM
- **Power System**: 12V battery + regulators for modules

---

## 🧰 Hardware Components

| Component              | Quantity | Role                     |
|------------------------|----------|--------------------------|
| STM32 Microcontroller  | 2        | Robot + Remote Controller|
| NRF24L01               | 2        | Wireless communication   |
| ESP32-CAM              | 1        | Video streaming          |
| Flame Sensor           | 1        | Fire detection           |
| MQ Gas Sensor          | 1        | Gas detection            |
| Oxygen Sensor          | 1        | Environmental monitoring |
| 800RPM Gear Motor      | 2+       | Locomotion               |
| Servo Motors (SG90/MG996R) | 5    | Robotic arm              |
| Joystick Module        | 1        | Movement control         |
| 10k Potentiometers     | 5        | Robotic arm control      |
| GSM Module (SIM800L)   | 1        | Alerts & messages        |
| High-Speed Fan         | 1        | Fire extinguishing       |
| Custom Remote PCB      | 1        | Manual control system    |

---

## 🔧 Software Tools Used

- STM32CubeMX / STM32CubeIDE
- Keil uVision
- Arduino IDE (for ESP32-CAM)
- EasyEDA / Altium Designer (for PCB)
- Proteus (Simulation, optional)
- GitHub (Version control)

---

## 📸 Robot Preview

> You can upload images or videos here showing your robot and remote in action.

---

## 🚀 Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/FireFighter-Robot-STM32-NRF24-ESP32CAM.git
2. Firmware

- Upload STM32 firmware (robot + remote) using STM32CubeIDE or Keil.

- Upload ESP32-CAM sketch from esp32-cam-code directory.

3.Hardware Setup

- Connect NRF24, servo motors, gas/flame/oxygen sensors to STM32 as per schematic.

- Power up using regulated 3.3V and 5V supplies.

- Ensure correct pin mappings as defined in the firmware.

🛠 Future Improvements
- Add obstacle avoidance using ultrasonic or LIDAR

- Include GPS for location tracking

- Battery level monitoring and auto-charging system

- Web interface for video feed and control

🙌 Contribution
Feel free to fork this project and contribute:

- Bug fixes

- Documentation

- Circuit design improvement

- Feature enhancements

📄 License
This project is open-source under the MIT License.

💬 Contact
For any queries or collaboration, contact:
Rajib Hasan
Email: RajibHasan.MTE@gmail.com
LinkedIn: Your LinkedIn Profile
