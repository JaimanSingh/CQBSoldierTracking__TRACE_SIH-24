# CQBSoldierTracking__TRACE_SIH-24
🚨 T.R.A.C.E — Tactical Reconnaissance and Communication Equipment
National Winner — Smart India Hackathon 2024 (NSG Problem Statement)

3D Live Soldier Tracking • Health Monitoring • Friend–Foe Detection • RL-based Route Optimization

⭐ STAR SUMMARY
S — Situation

Special forces needed a precise, reliable, GPS-independent indoor tracking system that works even when:

Power & WiFi are cut

GPS fails inside buildings

Multi-floor operations cause signal obstruction

Real-time health & identification are required

T — Task

Design a system that provides:

Exact 3D location across floors

Continuous health vitals

Friend–Foe identification

A fully independent mesh network

On-the-go deployment (no pre-installed infra)

🚀 A — Approach
1. Hardware Architecture

Armband (per soldier)

UWB module → precise 3D ranging

IMU (GA-50) → dead reckoning

ECG + vitals sensors → health tracking

ESP32 → wireless communication

Spektor Nodes (per floor)

Independent mesh network

ToF-based distance estimation

mmWave radar for person detection

Gateway Node

Collects data → Command Center

2. Localization & Communication Technique

UWB + ToF → stable ranging even with walls

SLAM + IMU fusion → continuity during signal loss

MIMO → improves spatial accuracy

Mesh Network → no dependency on WiFi/GPS/power supply

3. Command Center Dashboard (Software)

Live 3D mapping of all soldiers

Drag-and-drop soldier management

Health vitals view (ECG, HR)

Real-time alerts (unidentified person, SOS)

RL-based Chase Optimizer for pursuit routes

🙅‍♂️ Rejected Approaches (and Why)
Technology	Why We Didn’t Choose It
BLE	Highly unstable RSSI → inaccurate location
WiFi	Not available during operations; easy to jam
GPS	Fails indoors + gives only 2D location
Only Accelerometers	Drift increases → position becomes unusable
RFID Tags	Need line-of-sight; power-hungry
Altimeters	Unreliable due to weather/environment variations
🧠 R — Result

✔ Accurate 3D inter-floor soldier tracking

✔ Stable mesh network without external infrastructure

✔ Integrated health monitoring

✔ Working friend–foe detection prototype

✔ RL system produced chase path outputs

✔ Two deployment modes: pre-installed & throwable module

🏆 Won Smart India Hackathon 2024

📸 System Overview

Armband → UWB + IMU + ECG

Spektor Node → Mesh + mmWave + ToF

Gateway Node → Master receiver

Dashboard → Visualization + Analytics
