# CQBSoldierTracking__TRACE_SIH-24

# 🚨 T.R.A.C.E — Tactical Reconnaissance and Communication Equipment  
### **National Winner — Smart India Hackathon 2024 (NSG Problem Statement)**  

3D Live Soldier Tracking • Health Monitoring • Friend–Foe Detection • Reinforcement Learning (RL)–based Route Optimization  

---

## ⭐ STAR SUMMARY  

### **S — Situation**  
Special forces required a **precise, Global Positioning System (GPS)-independent indoor tracking system** for multi-floor operations where:  
- **GPS** fails  
- Power & WiFi are cut  
- Signals face obstruction from walls  
- Real-time health & identification are critical  

---

### **T — Task**  
Build a system capable of:  
- Accurate **3D soldier location**  
- **Health vitals tracking**  
- **Friend–Foe identification**  
- Working entirely on a **private mesh network**  
- **On-the-go deployment** without pre-installed infrastructure  

---

## 🚀 A — Approach  

### **1. Hardware Architecture**

#### **Armband (per soldier)**  
- **Ultra-Wideband (UWB)** module → precise 3D ranging  
- **Inertial Measurement Unit (IMU)** — GA-50 sensor → dead reckoning  
- **Electrocardiogram (ECG)** + vitals sensors → health monitoring  
- **ESP32 Microcontroller** → wireless communication  

#### **Spektor Nodes (per floor)**  
- Create independent **mesh network**  
- **Time of Flight (ToF)**–based ranging  
- **Millimeter-Wave (mmWave) Radar** for person detection  

#### **Gateway Node**  
- Aggregates floor-wise data  
- Sends to **Command Center Dashboard**  

---

### **2. Localization & Communication Stack**  
- **Ultra-Wideband (UWB)** for high-accuracy ranging  
- **Time of Flight (ToF)** to overcome reflections & obstruction issues  
- **Simultaneous Localization and Mapping (SLAM)** + **Inertial Measurement Unit (IMU)** fusion for continuous tracking  
- **Multiple Input Multiple Output (MIMO)** to enhance spatial precision  
- **Private Mesh Network** for complete independence from WiFi/GPS  

---

### **3. Command Center Software**  
- Real-time **3D soldier mapping**  
- Drag-and-drop for team allocation  
- Health monitoring (**Electrocardiogram – ECG**, Heart Rate – HR)  
- Unidentified person alerts  
- **Reinforcement Learning (RL)–based Chase Optimizer** for optimal pursuit routes  

---

## 🙅‍♂️ Rejected Approaches (and Why Not)

| Approach | Full Form | Reason Rejected |
|----------|-----------|-----------------|
| **BLE** | Bluetooth Low Energy | Highly unstable **Received Signal Strength Indicator (RSSI)** → poor distance accuracy |
| **WiFi** | Wireless Fidelity | Power/WiFi is shut down during operations |
| **GPS** | Global Positioning System | Fails indoors + only gives 2D location |
| **Only Accelerometers** | — | Position drift becomes unusable with time |
| **RFID Tags** | Radio-Frequency Identification | Requires line-of-sight; power-hungry |
| **Altimeters** | — | Weather/environment-dependent, inconsistent |

---

## 🧠 R — Result  
- ✔ Accurate **3D inter-floor soldier tracking**  
- ✔ Fully functional **mesh-based communication network**  
- ✔ Integrated **health vitals** (ECG, HR)  
- ✔ **Friend–Foe detection** prototype completed  
- ✔ **Reinforcement Learning (RL)** route optimizer output achieved  
- ✔ **Throwable / Pre-installation node deployment** options  
- 🏆 **Winner — Smart India Hackathon 2024** (NSG Problem Statement)  

---

## 📸 System Overview  
- **Armband:** Ultra-Wideband (UWB) + Inertial Measurement Unit (IMU) + Electrocardiogram (ECG)  
- **Spektor Node:** Mesh + Time of Flight (ToF) + Millimeter-Wave (mmWave) Radar  
- **Gateway:** Master receiver node  
- **Dashboard:** Visualization + Alerts + Data Monitoring  

---
 
