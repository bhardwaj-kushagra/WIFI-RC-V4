![70d6dc82-74ef-4aa7-a7a0-ac53ddcfa1ff](https://github.com/user-attachments/assets/719d8641-d014-4cb5-a8c4-e8b60a50cbca)
## Circuit Diagram (not mine obv.)

# 🚗 WiFi-Controlled RC Car with ESP32

## 📌 Overview
This project demonstrates how to build an **ESP32-based WiFi-controlled RC car** that can be operated via a web interface. By hosting a local IP-based webpage, users can remotely control the car's movement in real-time.

## 🔥 Features
- 📶 **WiFi-based Control** – Operate from any device connected to the same network.
- 🎮 **Web-Based Interface** – Control via browser buttons.
- ⚡ **Speed Control** – Adjust motor speed using a slider.
- 🔄 **Multi-Directional Movement** – Forward, backward, left, right.
- 🔋 **Separate Power Supply** – ESP32 and L298N powered independently for better efficiency.

## 🛠 Hardware Requirements
- ESP32 WiFi Development Board
- L298N Motor Driver Module
- 4 DC Motors + Wheels - I used BO Motors
- Breadboard & Jumper Wires
- 2x 1800mAh Batteries
- Battery Holder & Switch
- Android Arduino WiFi Car App

## 🔗 Circuit Connections
### **ESP32 Pins:**
| ESP32 | Component |
|-------|-----------|
| D5    | L298N IN1 |
| D6    | L298N IN2 |
| D7    | L298N IN3 |
| D8    | L298N IN4 |
| VIN   | Power (5V) |
| GND   | Ground |

### **L298N Motor Driver:**
| L298N | Component |
|-------|-----------|
| OUT1  | Motor 1 |
| OUT2  | Motor 2 |
| OUT3  | Motor 3 |
| OUT4  | Motor 4 |
| 12V   | Battery Positive |
| GND   | Battery & ESP32 GND |

## 🚀 How It Works
1. The **ESP32 connects to WiFi** and generates a local IP.
2. The **web interface** (hosted on ESP32) loads in the browser.
3. Users send commands via **web buttons** to control movement.
4. The ESP32 processes signals and drives **L298N motor controller**.
5. The car responds to user input and executes **directional movement**.

## 📡 Web Interface
The car is controlled via a simple **HTML webpage** hosted by the ESP32. Open the **ESP32's IP in a browser**, and use buttons to navigate the car.

## 🔧 Setup Instructions
1. Assemble the car **chassis, motors, and wheels**.
2. Connect motors to **L298N motor driver**.
3. Wire the **ESP32 to L298N** as per the connection table.
4. Upload the **Arduino code** to ESP32 (ensure WiFi credentials are correct).
5. Power the car and **open the IP address** in a browser.
6. Control the car using the **web buttons**!

## 🔮 Future Improvements
- 🛣 **Obstacle Avoidance** using **Ultrasonic Sensors**.
- 📱 **Mobile App** instead of web control.
- 🎤 **Voice Commands** for hands-free operation.
- 🔄 **Path Following** using **line-tracking sensors**.

## 💡 Conclusion
This project combines **IoT, robotics, and web development** to create a **smart, remote-controlled car**. It provides hands-on experience with **ESP32, motor drivers, and WiFi-based automation**. 🚗💨 Happy coding!

---
### 📜 License
This project is open-source under the **MIT License**.



