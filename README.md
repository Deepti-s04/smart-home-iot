# 💡 Smart Home IoT Project

A simple and secure IoT system that allows users to control an LED from a web interface using **ESP32**, **AWS IoT Core**, and **Arduino**.

---

## 🔧 Features

- ON/OFF control of LED via web interface
- Real-time communication using **MQTT**
- AWS IoT Core used as cloud bridge
- Secure connection using certificates
- Website hosted on **AWS S3**

---

## 🚀 Technologies Used

- HTML, CSS, JavaScript (Frontend)
- ESP32 (IoT device)
- Arduino IDE (Programming ESP32)
- AWS IoT Core (MQTT Broker)
- AWS API Gateway + Lambda (Backend)
- AWS S3 (Hosting Website)

---

## 🌐 Live Demo

**[👉 Open Website](http://smart-home-website.s3-website.eu-north-1.amazonaws.com)**  
Control your LED from anywhere through the internet.

---

## 🔌 How It Works

1. Website sends LED ON/OFF request to AWS API Gateway.
2. API Gateway triggers a Lambda function.
3. Lambda function publishes the command to **AWS IoT Core** MQTT topic.
4. ESP32, subscribed to that topic, receives the message and toggles the LED.

---
