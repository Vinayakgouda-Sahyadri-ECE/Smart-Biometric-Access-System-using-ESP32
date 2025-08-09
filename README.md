# Smart Biometric Access System using ESP32

A secure **fingerprint-based access control system** built with an **ESP32** and **R307 fingerprint sensor**.  
Includes a custom **web portal** for real-time logging, manager-level controls, and user authorization.  
Designed with a focus on **automation**, **data security**, and **IoT-based access management**.

---

## 📌 Features
- Fingerprint authentication using **R307 Sensor**
- Real-time entry/exit logging
- Web-based dashboard with:
  - Log viewing for managers
  - User authorization controls
- Access control with LED and buzzer feedback
- Secure username/password login for portal
- On-device log storage using SPIFFS
- Time synchronization via NTP

---

## 🛠 Tools & Technologies
- **ESP32**
- **R307 Fingerprint Sensor**
- **Web Interface** (ESP32 WebServer)
- **Arduino IDE**

---

## 📂 Hardware Requirements
- ESP32 development board
- R307 fingerprint sensor
- LED (with resistor)
- Buzzer
- Jumper wires
- Breadboard or PCB

---

## 📂 Software Requirements
- Arduino IDE with ESP32 board package
- Libraries:
  - [`Adafruit_Fingerprint`](https://github.com/adafruit/Adafruit-Fingerprint-Sensor-Library)
  - `WiFi.h`
  - `WebServer.h`
  - `FS.h` & `SPIFFS.h`
  - `time.h`

---

## 🚀 How It Works
1. The ESP32 connects to Wi-Fi and initializes the fingerprint sensor.
2. A registered user places their finger on the R307 sensor.
3. If authenticated:
   - Access is granted
   - Logs are stored with timestamp
   - LED and buzzer provide feedback
4. If authentication fails, an alert beep is triggered.
5. Managers can log in to the web dashboard to view logs and manage access.

---

## 🌐 Web Portal
- Access by entering the ESP32's IP address in a browser.
- Default Login:
  - Admin: `admin` / `1234`
  - Guest: `guest` / `5678`
- View logs in chronological order
- Logout option for session security

---


