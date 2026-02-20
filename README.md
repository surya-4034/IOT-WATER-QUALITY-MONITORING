🌊 IoT-Based Water Quality Monitoring System
Using ESP32 & TDS Sensor with ThingSpeak Cloud
________________________________________
📌 Project Overview
This project presents an IoT-Based Water Quality Monitoring System developed using the ESP32 microcontroller and a Total Dissolved Solids (TDS) sensor. 
The system continuously measures the TDS level of water and uploads the data to the cloud platform ThingSpeak for real-time monitoring and visualization.
The main objective of this project is to provide a low-cost, reliable, and real-time solution for monitoring water quality remotely using IoT technology.
________________________________________
🎯 Objectives

•	To measure water quality using a TDS sensor

•	To process sensor data using ESP32

•	To transmit real-time data to the cloud

•	To enable remote monitoring through a web dashboard

•	To reduce manual water testing efforts
________________________________________
🛠️ Hardware Components

•	ESP32 Development Board


<img width="300" height="300" alt="Screenshot 2026-02-21 015723" src="https://github.com/user-attachments/assets/437bf549-37ba-42ee-a312-a03f801e0c61" />

•	TDS Sensor Module

<img width="327" height="243" alt="Screenshot 2026-02-21 015802" src="https://github.com/user-attachments/assets/79baf5b4-2fd1-4be1-b8d2-0d33c6db8fee" />

•	Jumper Wires

<img width="234" height="250" alt="Screenshot 2026-02-21 020508" src="https://github.com/user-attachments/assets/47c5e8a2-ae51-4f08-bc46-b962c10faadd" />

•	USB Cable (Power Supply)
•	Wi-Fi Internet Connection
________________________________________
💻 Software Requirements
•	Arduino IDE (Version 1.8.19 Recommended)

•	ESP32 Board Package Installed

•	Required Libraries:

o	WiFi.h

o	ThingSpeak.h

•	ThingSpeak Account (Channel & API Key)
________________________________________
🧠 Working Principle
The system works based on the electrical conductivity of water. Dissolved salts and minerals increase the conductivity of water, which directly relates to the TDS value.
1.	The TDS probe is immersed in the water sample.
2.	The sensor generates an analog voltage based on conductivity.
3.	ESP32 reads the analog signal using its ADC.
4.	The signal is converted into TDS value (ppm).
5.	Data is displayed on the Serial Monitor.
6.	The ESP32 sends the data to ThingSpeak via Wi-Fi.
7.	The cloud dashboard displays real-time graphs.
________________________________________
🔌 Circuit Connections
TDS Sensor Pin	ESP32 Pin
VCC	3.3V / 5V
GND	GND
AOUT	GPIO 34 (Analog Input)
Ensure proper grounding for stable readings.
<img width="405" height="198" alt="Screenshot 2026-02-21 004319" src="https://github.com/user-attachments/assets/7fca7b73-4fac-4f86-8209-0111e5f2daa2" />

________________________________________
☁️ Cloud Integration (ThingSpeak Setup)
1.	Create an account on ThingSpeak.
2.	Create a new channel.
3.	Add a field (e.g., "TDS Value").
4.	Copy the Write API Key.
5.	Add the API key in your Arduino code.
6.	Upload code to ESP32.
7.	Monitor live data on the dashboard.
Note: ThingSpeak updates data every 15 seconds (minimum interval).
________________________________________
📊 TDS Water Quality Reference
TDS (ppm)	Water Quality
<img width="600" height="600" alt="Screenshot 2026-02-21 015454" src="https://github.com/user-attachments/assets/2aeab84b-2abe-4e8d-b718-6ed5c83ea7e1" />

________________________________________
🧪 Testing Procedure
•	Dipped probe in water sample

•	Verified readings on Serial Monitor

•	Checked Wi-Fi connectivity

•	Confirmed data upload to ThingSpeak

•	Observed real-time graphical display

System successfully measured and transmitted water quality data.

<img width="500" height="500" alt="Screenshot 2026-02-21 011444" src="https://github.com/user-attachments/assets/f594a6b2-bf4a-4bdf-8d6f-71c93e9f4536" />



________________________________________
🚀 Features
   •	Real-time monitoring 

  •	Wireless data transmission

  •	Cloud storage and visualization

  •	Low-cost IoT implementation

  •	Easy to deploy
________________________________________
🔮 Future Scope
  •	Add pH, turbidity, and temperature sensors

  •	Develop mobile app with alert system

  •	Implement SMS/email notifications

  •	Add solar power for remote deployment

  •	Integrate machine learning for trend prediction

  •	Expand for industrial and smart city use
________________________________________
📚 References
   •	ThingSpeak Official Documentation
 
  •	Arduino IDE

  •	ESP32 Datasheet – Espressif Systems

  •	TDS Sensor Datasheet

  •	ChatGPT – Documentation guidance

  •	YouTube – Implementation tutorials
________________________________________
🏁 Conclusion
This project demonstrates a practical implementation of IoT in environmental monitoring. The ESP32-based water quality monitoring system effectively measures TDS levels and uploads data to the cloud for remote access.
It provides a reliable, scalable, and cost-effective solution for smart water management and contributes toward sustainable environmental monitoring systems.
________________________________________
📎 License
This project is open-source and available for educational and research purposes.

