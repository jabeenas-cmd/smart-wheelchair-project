# ♿ Smart Voice & Gesture Controlled Wheelchair

A smart wheelchair powered by ESP32 with voice and gesture control, real-time IoT monitoring, and advanced safety features for hands-free and secure navigation.

---

## 🚀 Features

### 🎤 Voice Control
- Control wheelchair using voice commands  
- Supported commands:
  - Forward, Backward, Left, Right, Stop  
  - Emergency Stop  
  - Light ON / OFF  
- Works **offline** (no internet required)  
- Emergency command instantly stops the wheelchair and sends alert  

---

### ✋ Gesture Control
- Controlled using hand tilt (MPU6050 sensor)  
- Movements:
  - Tilt Forward → Move Forward  
  - Tilt Back → Move Backward  
  - Tilt Left → Turn Left  
  - Tilt Right → Turn Right  
  - No tilt → Stop  
- Works when voice control is inactive  

---

### 🚧 Obstacle Detection
- Uses **two ultrasonic sensors** (Front & Back)

**Front Sensor:**
- Detects obstacles ahead  
- Stops forward & turning movement if obstacle is too close  

**Back Sensor:**
- Detects obstacles behind  
- Stops backward movement if obstacle is too close  

✔ Prevents collisions and ensures safe navigation  

---

### 🔊 Buzzer Alert System
- Alerts user when obstacle is nearby  
- Buzzer ON if:
  - Front distance < 20 cm  
  - OR Back distance < 20 cm  
- Works even when wheelchair is not moving  
- Turns OFF when path is clear  

---

### 📱 IoT Monitoring (Blynk)
- Connected via WiFi using ESP32  
- Real-time monitoring through mobile app  

**Displays:**
- Wheelchair movement status  
  - Forward / Backward / Left / Right / Stopped  
- Front obstacle distance  
- Back obstacle distance  

✔ Enables remote monitoring by user/caretaker  

---

### 🚨 Emergency Alert System
- Triggered using voice command  
- Instantly:
  - Stops wheelchair  
  - Sends alert notification via Blynk  

---

### ⚙️ RTOS-Based System
- Built using Real-Time Operating System (RTOS)  
- Handles multiple tasks simultaneously:
  - Voice processing  
  - Gesture control  
  - Obstacle detection  
  - IoT communication  

✔ Ensures fast response and smooth operation  

---

### 🧠 Smart Control Logic
- Voice control has highest priority  
- Gesture control works only when voice is inactive  
- Obstacle detection overrides all controls for safety  

---

## 🛠️ Hardware Used
- ESP32 Microcontroller  
- VC-02 Voice Recognition Module  
- MPU6050 Accelerometer & Gyroscope  
- Ultrasonic Sensors (Front & Back)  
- Motor Driver  
- Buzzer  
- Wheels & Chassis  

---

## 💻 Software Used
- Embedded C  
- ESP32 Programming  
- FreeRTOS  
- Blynk IoT Platform  

---

## 📊 System Working
The ESP32 acts as the central controller managing all sensors and modules.  
Using RTOS, multiple operations like voice control, gesture control, obstacle detection, and IoT communication run in parallel.  

This ensures:
- Fast response  
- Smooth navigation  
- Reliable performance  

---

## 📱 IoT Dashboard Parameters
- **V0:** Wheelchair Status  
- **V1:** Front Obstacle Distance (cm)  
- **V2:** Back Obstacle Distance (cm)  

---

## 🎯 Applications
- Assistive mobility for physically challenged individuals  
- Hospitals and rehabilitation centers  
- Elderly care systems  

---

## 👩‍💻 Developed By
**Jabeena Shaik**  
B.Tech – Electronics & Communication Engineering  
---
