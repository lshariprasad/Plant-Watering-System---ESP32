🌱 Plant Watering System — ESP32

Smart · Wireless · Self-Managing Irrigation

Welcome to the Plant-Watering-System — ESP32, a fully automated, IoT-enabled irrigation controller designed to keep your plants healthy even when you're away.
Built on the power of the ESP32, this system monitors soil moisture and activates a water pump only when required—saving water, time, and effort.

🚀 Features
✔ Automatic Watering

The ESP32 reads soil moisture and activates the motor automatically.

✔ Manual Watering Control (Web Dashboard)

Trigger the pump manually through a mobile-friendly webpage.

✔ Live Monitoring

Real-time soil moisture percentage displayed on the dashboard.

✔ WiFi-Based Control

No apps. No Bluetooth.
Just connect to ESP32’s Access Point → Open the webpage → Control.

✔ Safe Motor Control

Uses relay or motor driver for safe pump switching.

🧠 System Architecture
[Soil Moisture Sensor] → ESP32 → [Motor Driver / Relay] → Water Pump
                                   ↑
                                   |
                           Web Dashboard (WiFi)

🛠 Hardware Components

ESP32 Dev Module / ESP32 Cam

Soil Moisture Sensor (Analog / Capacitive)

Relay / L298N Motor Driver

Water Pump (5V/12V)

Power Supply / Battery

📂 Project Structure
Plant-Watering-System---ESP32/
│── src/
│    └── main.cpp         # Core logic
│── web/
│    └── index.html       # Control dashboard
│── assets/
│    └── images           # System diagrams (optional)
│── README.md             # You are here

🔌 Wiring Overview
Component	ESP32 Pin
Soil Sensor OUT	GPIO 34 (ADC)
Relay IN	GPIO 26
Water Pump	Relay Output
5V Supply	VIN / 5V
GND	GND
🌐 Web Dashboard Preview

Toggle pump ON/OFF

View:

Soil moisture %

Pump status

Last watering time

🧩 How It Works
1️⃣ Read Moisture

ESP32 reads analog value from soil sensor → converts it to %.

2️⃣ Decision Making

If moisture < threshold → pump ON
If moisture > threshold → pump OFF

3️⃣ Remote Control

User can override automatic mode via web dashboard.

4️⃣ Data Update

Moisture data refreshes every second.

🧪 Future Enhancements

🌦️ Add weather API (skip watering when it rains)

📶 Send notifications to mobile

🌿 Integrate multiple plant zones

🎤 Add voice control (Alexa / Google)

⚡ Use deep sleep for low power mode

👨🏻‍💻 Developer

Created by Hari (Dev)
A smart automation project built for effortless and reliable plant care.

⭐ If you like this project…

Help the repo grow:
Star ⭐ this repository — it motivates further upgrades!
