# CQBSoldierTracking__TRACE_SIH-24
# 🚨 T.R.A.C.E — Tactical Reconnaissance and Communication Equipment  
### **National Winner — Smart India Hackathon 2024 (NSG Problem Statement)**  

3D Live Soldier Tracking • Health Monitoring • Friend–Foe Detection • RL-based Route Optimization  

---

## ⭐ STAR SUMMARY  

### **S — Situation**  
Special forces required a **precise, GPS-independent indoor tracking system** for multi-floor operations where:  
- GPS fails  
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
- **On-the-go deployment** without pre-installed infra  

---

## 🚀 A — Approach  

### **1. Hardware Architecture**

#### **Armband (per soldier)**  
- UWB module → precise 3D ranging  
- IMU (GA-50) → dead reckoning  
- ECG + vitals sensors → health monitoring  
- ESP32 → wireless communication  

#### **Spektor Nodes (per floor)**  
- Create independent mesh network  
- Time-of-Flight (ToF)-based ranging  
- mmWave radar for person detection  

#### **Gateway Node**  
- Aggregates floor-wise data  
- Sends to Command Center Dashboard  

---

### **2. Localization & Communication Stack**  
- **Ultra-Wideband (UWB)** for high-accuracy ranging  
- **ToF (Time of Flight)** to overcome reflections & obstruction issues  
- **SLAM + IMU fusion** to maintain location even with signal loss  
- **MIMO** to enhance spatial precision  
- **Private Mesh Network** for complete independence from WiFi/GPS  

---

### **3. Command Center Software**  
- Real-time **3D soldier mapping**  
- Drag-and-drop for team allocation  
- Health monitoring (ECG, HR)  
- Unidentified person alerts  
- **RL-based Chase Optimizer** for optimal pursuit routes  

---

## 🙅‍♂️ Rejected Approaches (and Why Not)

| Approach | Reason Rejected |
|----------|-----------------|
| **BLE** | Unstable RSSI → poor distance accuracy |
| **WiFi** | Power/WiFi is shut down during operations |
| **GPS** | Fails indoors + only gives 2D location |
| **Only Accelerometers** | Position drift becomes unusable over time |
| **RFID Tags** | Line-of-sight only; high power requirement |
| **Altimeters** | Weather-dependent & inconsistent |

---

## 🧠 R — Result  
- ✔ **Accurate 3D inter-floor tracking**  
- ✔ Fully functional **mesh-based communication**  
- ✔ **Health vitals integration**  
- ✔ **Friend–Foe detection** prototype completed  
- ✔ **RL route optimizer** output achieved  
- ✔ **Throwable / Pre-installation node deployment** options  
- 🏆 **Winner — Smart India Hackathon 2024** (NSG Problem Statement)  

---

## 📸 System Overview  
- **Armband:** UWB + IMU + ECG  
- **Spektor Node:** Mesh + ToF + mmWave  
- **Gateway:** Master receiver  
- **Dashboard:** Visualization + Alerts  

---

## 🧩 Recommended Repository Structure  
