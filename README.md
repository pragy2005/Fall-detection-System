# 🛡️ Fall Detection System

This project is a real-time **Fall Detection System** designed to monitor human motion using sensors and alert caregivers in case of a fall. It utilizes an **ESP8266 NodeMCU** microcontroller and an **MPU6050 (accelerometer + gyroscope)** sensor to detect unusual movement patterns indicating a fall.

---

## 📌 Features

- 📡 Real-time fall detection using MPU6050
- 🔔 Sends alerts to a mobile phone via Wi-Fi
- 📈 Captures and analyzes acceleration and orientation data
- 💡 Lightweight and power-efficient, suitable for wearable devices
- 🛠️ Can be integrated with mobile apps or cloud services (like Blynk, IFTTT, Firebase, etc.)

---

## 🧰 Hardware Requirements

- 🔌 ESP8266 NodeMCU
- 📟 MPU6050 (Accelerometer + Gyroscope)
- 🔋 Power source (e.g., battery or USB)
- 📱 Wi-Fi connection
- 🧪 Optional: Buzzer, LED, or alert module for local warnings

---

## 🔧 How It Works

1. The MPU6050 constantly sends acceleration and gyroscope data to the ESP8266.
2. A fall is detected when sudden, abnormal values are registered (like a free fall or sharp tilt).
3. If a fall is detected, the ESP8266 sends an alert via Wi-Fi to a connected phone or server.
4. Optional: Add delay/timer before sending alert to allow user to cancel if false positive.

---

## 💻 Software Setup

### 1. Libraries Required (Arduino IDE)

- `Wire.h`
- `ESP8266WiFi.h`
- `Adafruit_MPU6050.h`
- `Adafruit_Sensor.h`

### 2. Uploading Code

- Connect ESP8266 via USB
- Select correct port and board in Arduino IDE
- Upload the code from `fall_detection.ino`

---

## 📱 Alert Methods (Choose one)

- **Blynk App**
- **IFTTT Webhooks**
- **SMS/Email via Firebase or custom backend**
- **Telegram Bot / Pushbullet integration**

> You can customize the notification logic in the code based on your preferred method.

---

## 📷 Demo

*Insert a screenshot, serial monitor output, or GIF here showing a detected fall and alert sent.*

---

## ⚠️ Limitations

- May detect false positives from sudden movements (jumping, sitting fast)
- Requires stable Wi-Fi for notification
- Threshold values might need calibration for different users

---

## 🧪 Future Improvements

- AI/ML model to improve accuracy
- Battery optimization for wearables
- Fall confirmation via user response before alerting
- Cloud logging for caregivers

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 🙋‍♂️ Author

Developed by **[Your Name]**  
Originally uploaded on another account, now maintained here.

Feel free to contribute or raise issues!

