🌊 IoT-Based Water Quality Monitoring System
Using ESP32 & TDS Sensor with ThingSpeak Cloud
📌 Project Overview

This project presents an IoT-Based Water Quality Monitoring System developed using the ESP32 microcontroller and a Total Dissolved Solids (TDS) sensor. The system continuously measures the TDS level of water and uploads the data to the cloud platform ThingSpeak for real-time monitoring and visualization.

The main objective of this project is to provide a low-cost, reliable, and real-time solution for monitoring water quality remotely using IoT technology.

🎯 Objectives

To measure water quality using a TDS sensor
To process sensor data using ESP32
To transmit real-time data to the cloud
To enable remote monitoring through a web dashboard
To reduce manual water testing efforts

🛠️ Hardware Components

ESP32 Development Board

TDS Sensor Module

Jumper Wires

Breadboard

USB Cable (Power Supply)

Wi-Fi Internet Connection

💻 Software Requirements

Arduino IDE (Version 2.x Recommended)

ESP32 Board Package Installed

Required Libraries:

WiFi.h

ThingSpeak.h

ThingSpeak Account (Channel & API Key)

🧠 Working Principle

The system works based on the electrical conductivity of water. Dissolved salts and minerals increase the conductivity of water, which directly relates to the TDS value.

The TDS probe is immersed in the water sample.

The sensor generates an analog voltage based on conductivity.

ESP32 reads the analog signal using its ADC.

The signal is converted into TDS value (ppm).

Data is displayed on the Serial Monitor.

The ESP32 sends the data to ThingSpeak via Wi-Fi.

The cloud dashboard displays real-time graphs.

🔌 Circuit Connections
TDS Sensor Pin	ESP32 Pin
VCC	3.3V / 5V
GND	GND
AOUT	GPIO 34 (Analog Input)

Ensure proper grounding for stable readings.

☁️ Cloud Integration (ThingSpeak Setup)

Create an account on ThingSpeak.

Create a new channel.

Add a field (e.g., "TDS Value").

Copy the Write API Key.

Add the API key in your Arduino code.

Upload code to ESP32.

Monitor live data on the dashboard.

Note: ThingSpeak updates data every 15 seconds (minimum interval).

📊 TDS Water Quality Reference
TDS (ppm)	Water Quality
0–50	Very Pure
50–150	Excellent
150–300	Good
300–500	Fair
500–1000	Poor
Above 1000	Unsafe
🧪 Testing Procedure

Dipped probe in water sample

Verified readings on Serial Monitor

Checked Wi-Fi connectivity

Confirmed data upload to ThingSpeak

Observed real-time graphical display

System successfully measured and transmitted water quality data.

🚀 Features

Real-time monitoring

Wireless data transmission

Cloud storage and visualization

Low-cost IoT implementation

Easy to deploy

🔮 Future Scope

Add pH, turbidity, and temperature sensors

Develop mobile app with alert system

Implement SMS/email notifications

Add solar power for remote deployment

Integrate machine learning for trend prediction

Expand for industrial and smart city use

📚 References

ThingSpeak Official Documentation

Arduino IDE

ESP32 Datasheet – Espressif Systems

TDS Sensor Datasheet

ChatGPT – Documentation guidance

YouTube – Implementation tutorials

🏁 Conclusion

This project demonstrates a practical implementation of IoT in environmental monitoring. The ESP32-based water quality monitoring system effectively measures TDS levels and uploads data to the cloud for remote access.

It provides a reliable, scalable, and cost-effective solution for smart water management and contributes toward sustainable environmental monitoring systems.

📎 License

This project is open-source and available for educational and research purposes.
