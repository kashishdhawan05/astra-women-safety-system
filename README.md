# astra-women-safety-system
Of🚨 ASTRA – Smart Women Safety System (Offline IoT Device)

⚡ Designed for critical situations where speed, reliability, and independence from smartphones matter the most.

An embedded safety solution that ensures instant emergency alerts with location tracking, without relying on internet connectivity.

🌍 Motivation

In real-world emergencies, delays caused by unlocking phones, opening apps, or lack of internet can be dangerous.

Most safety systems today:

Depend heavily on mobile devices

Require multiple user interactions

Fail under poor connectivity

This system is built to remove these dependencies entirely.

🚨 Problem Overview

Safety challenges become more serious in:

Low-network or rural regions

Situations where phone access is not possible

High-stress scenarios requiring immediate action

Existing app-based solutions are often unreliable in such conditions.

💡 System Approach

This project introduces a dedicated hardware-based safety device that:

Operates independently of smartphones

Sends SMS alerts with precise GPS location

Activates instantly using a single button

Maintains functionality in weak signal environments

⚙️ Operational Flow

SOS button is triggered

Device wakes from standby mode

GPS module locks location (~3–5 seconds)

ESP32 processes coordinates

GSM module transmits SMS with location link

Emergency contact receives alert

🆚 Existing vs Proposed System
Parameter	App-Based Systems	ASTRA Device
Internet Required	Yes	❌ No
Response Time	Moderate	⚡ Fast
Reliability	Variable	High
Ease of Use	Multi-step	✅ Single tap
🧠 Design Considerations

⚡ Fast response time (under 10 seconds)

🔋 Optimized power usage with standby mode

📡 GSM-based communication for wider coverage

🔁 Stable and repeatable alert mechanism

🛡️ System Reliability

No dependency on internet services

Minimal user interaction required

Works in high-stress environments

Designed for consistent SMS delivery

🧰 Hardware Setup

ESP32 Development Board

NEO-6M GPS Module

GSM Module (SIMCOM / A7670)

OLED Display (I2C Interface)

Rechargeable Li-ion Battery

Charging Module (TP4056)

🔌 Pin Configuration
Component	ESP32 Pin
GPS TX	GPIO16
GPS RX	GPIO17
GSM TX	GPIO26
GSM RX	GPIO27
SOS Switch	GPIO4
📊 System Performance

⏱️ Alert Trigger Time: 5–10 seconds

📍 Location Accuracy: ~3m (open), ~6m (urban)

🔋 Standby Backup: Up to 72 hours

✅ SMS Success Rate: Reliable under testing

🖼️ Prototype Implementation

🎥 Demonstration

(Add demo video link here)

💻 Codebase
firmware/esp32_code/safety_system.ino
📄 Documentation

Research Paper: docs/research_paper.pdf

Circuit Design: docs/circuit_diagram.png

🧪 Testing Conditions

The system was evaluated under:

Weak GSM network conditions

Outdoor and dense urban environments

Multiple emergency trigger scenarios

Stable and repeatable results were achieved.

🚀 Future Scope

Integration with mobile dashboard

Real-time tracking via cloud

Miniaturized wearable version

Intelligent auto-trigger system

⚡ Key Highlights

Fully offline operation

Faster response than mobile solutions

Works in low connectivity areas

Simple one-button activation

👩‍💻 Developer
🔹 Kashish Dhawan

System Design & Research

Embedded System Development

📬 Connect

(Open for collaboration, improvements, and real-world deployment discussions)fline IoT-based women safety device using ESP32, GPS, and GSM
