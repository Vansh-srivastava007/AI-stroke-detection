#  Hybrid Stroke Risk Monitoring System

![IoT](https://img.shields.io/badge/Type-IoT-blue)
![AI](https://img.shields.io/badge/Model-ML-green)
![Backend](https://img.shields.io/badge/Backend-Flask-black)
![Status](https://img.shields.io/badge/Status-Active-success)
![License](https://img.shields.io/badge/Purpose-Educational-orange)

A full-stack IoT + AI system that predicts stroke risk in real time by combining clinical patient data with live physiological sensor inputs.

This project integrates **embedded systems, machine learning, cloud computing, and real-time streaming** into a scalable monitoring architecture.

---

##  Table of Contents

- Overview  
- System Architecture  
- How It Works  
- Tech Stack  
- Project Structure  
- Deployment  
- Key Features  
- Disclaimer  

---

##  Overview

The system continuously evaluates stroke risk using:

- 🩺 Clinical data (age, hypertension, heart disease, glucose, BMI)
- 📡 Live sensor data (BPM, ECG, temperature)
- 🤖 Machine learning prediction model
- 🌐 Cloud-hosted backend
- 📊 Real-time web dashboard
- 📟 OLED edge display

---

##  System Architecture

ESP32 (Sensors + OLED)
│
▼
Cloud Backend (Flask + ML + WebSocket)
│
▼
Web Dashboard (Real-Time Monitoring)

---

##  How It Works

1. Patient clinical profile is entered via the dashboard.
2. ESP32 continuously collects physiological data.
3. Sensor data is sent to the cloud backend.
4. Backend merges clinical + sensor inputs.
5. ML model predicts stroke risk probability.
6. Risk score is:

   - Displayed on OLED (edge device)
   - Streamed live to dashboard
   - Stored in database

---

##  Tech Stack

### 🔹 Hardware
- ESP32
- AD8232 ECG Sensor
- Pulse Sensor
- Temperature Sensor
- OLED (SSD1306)

### 🔹 Backend
- Flask  
- Flask-SocketIO  
- SQLAlchemy  
- Scikit-learn  
- Docker  
- Render (Cloud Hosting)

### 🔹 Frontend
- HTML + CSS 
- Chart.js  
- Vercel (Deployment)

### 🔹 Machine Learning
- RandomForest / Scikit-learn  
- StandardScaler  
- Hybrid feature model (clinical + sensor)

---

## 📁 Project Structure

stroke-ai-system/
│
├── backend/
├── dashboard/
├── firmware/
└── README.md

**backend/** → API, ML inference, database, WebSocket  
**dashboard/** → Real-time monitoring interface  
**firmware/** → ESP32 code  

---

##  Deployment

- Backend deployed on **Render**
- Dashboard deployed on **Vercel**
- Dockerized backend for portability

---

## 🎯 Key Features

✔ Hybrid clinical + real-time monitoring  
✔ Cloud-based ML inference  
✔ WebSocket real-time updates  
✔ Edge-level OLED alerts  
✔ Scalable architecture  
✔ Containerized deployment  

---



 **If you like this project, consider starring the repository!**
