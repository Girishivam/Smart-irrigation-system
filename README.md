
# Smart-irrigation-System-
# 🌿 Automatic Smart Irrigation System

<p align="center">

[![Author: Ankur Gupta](https://img.shields.io/badge/Author-Ankur%20Gupta-blue?style=flat-square)](https://example.com)
[![Author: Harshit Gupta](https://img.shields.io/badge/Author-Harshit%20Gupta-green?style=flat-square)](https://example.com)
[![Author: Shivam Giri](https://img.shields.io/badge/Author-Shivam%20Giri-red?style=flat-square)](https://example.com)
[![Author: Abhinav Raj](https://img.shields.io/badge/Author-Abhinav%20Raj-orange?style=flat-square)](https://example.com)
[![Author: Parth Gupta](https://img.shields.io/badge/Author-Parth%20Gupta-yellow?style=flat-square)](https://example.com)

</p>

An open‑source automatic irrigation system that measures soil moisture and water depth, then triggers watering only when needed...

...
## 📸 Parts Used

<div align="center">
  <img alt="Portfolio Demo" src="./Media/Parts used  in my project.png" />
</div>


## 🔍 Objective
- Automate irrigation to save time, water, and energy  
- Deploy a scalable prototype with minimal human intervention  
- Modular design for easy future enhancements  
- Enable remote monitoring and data logging  

## 🛠️ Hardware Components
- Arduino Uno  
- NodeMCU (ESP8266)  
- DS1307 RTC module  
- Soil moisture sensor  
- Water depth sensor  
- 5 V single-channel relay  
- 16×2 LCD display  
## 📸 Circuit Diagram

<div align="center">
  <img alt="Portfolio Demo" src="./Media/circuit.png" />
</div>
## 💾 Software Tools
- Arduino IDE  
- ThingSpeak account (READ + WRITE API keys)

---

## 📌 Wiring Diagram

### RTC → Arduino
- VCC → 5 V, GND → GND, SDA → SDA, SCL → SCL  

### LCD → Arduino
- 1 (GND) → GND  
- 2 (5 V) → 5 V  
- 3 (CONTRAST) → D10  
- 4 → D12 | 5 → GND | 6 → D11  
- 11 → D5 | 12 → D4 | 13 → D3 | 14 → D2  
- 15 → 5 V | 16 → GND  

### Soil Moisture Sensor → A0  
### Water Depth Sensor → A1  
- VCC → 5 V, GND → GND  

### Relay (Pump Control)
- IN → D8, VCC → 5 V, GND → GND  
- Pump: COM → Relay output, GND → GND  

### NodeMCU → Arduino
- VIN → 5 V, GND → GND  
- D1 → D0 | D2 → D1 | D3 → D7  

---

## 🧩 Configuration Steps

1. **Set soil & water thresholds** based on plant needs.  
2. **Schedule watering** (e.g., early morning) with RTC.  
3. **ThingSpeak setup**: Add Wi‑Fi SSID/password, Channel ID, and API keys in the NodeMCU code.

---

## 🚀 How It Works
1. RTC triggers system at scheduled time  
2. Arduino reads soil/moisture and water depth sensors  
3. Data displays on the LCD  
4. If thresholds are met, relay activates the pump  
5. NodeMCU uploads readings to ThingSpeak for remote monitoring  

---

## 📡 Remote Monitoring
View real-time and historical data on your ThingSpeak dashboard.

---

## 📦 How to Use

1. Clone the repo  
2. Open `smart_irrigation.ino` in Arduino IDE  
3. Update Wi‑Fi and ThingSpeak credentials  
4. Upload code to Arduino and NodeMCU  
5. Power the system and monitor via LCD or ThingSpeak  

---

## 📋 License
This project is **MIT‑licensed** — feel free to use and adapt.

---

## 🙏 Attribution
If you adapt this project, please credit the authors listed above in your documentation. 😊
