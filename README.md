# 🌐 Cloud-based IoT System Simulation Project
# IoT MQTT Simulation – CIS600 Assignment 3

This project simulates a virtual environmental station that collects data from temperature, humidity, and CO₂ sensors, and publishes this data to a ThingSpeak channel using the MQTT protocol.

It was completed as part of **CIS600 : Internet of Things - Application Development (Spring 2025)**.

---

## 📦 Project Files

| File Name | Description |
|-----------|-------------|
| `mqtt_thingspeak_publisher.py` | Simulates virtual sensor data (Temperature, Humidity, CO₂) and publishes it to ThingSpeak every 15 seconds using MQTT. Also logs the data locally in `sensor_log.txt`. |
| `last_5_hour_data.py` | Parses `sensor_log.txt` and prints data for a selected sensor from the last 5 hours. |
| `sensor_log.txt` | Auto-generated file storing timestamped sensor readings locally. |
| `vpalapar_Assignment_3_IoT_App_Dev.pdf` | Final submission pdf file with the brief explanation, screenshots, and reflection. |

---

## 📡 Technologies Used

- **Python 3**
- **ThingSpeak (MQTT & REST API)**
- **paho-mqtt** (for MQTT communication)
- **Local File Logging** (for historical analysis)

---

## 🚀 How It Works

1. **ThingSpeak Setup**  
   - A channel named `Environmental Station` was created with 3 fields (Temperature, Humidity, CO₂).
   - An MQTT device `VirtualStation1` was configured and linked to the channel.

2. **Data Publishing**  
   - `mqtt_thingspeak_publisher.py` simulates random data and sends it to ThingSpeak every 15 seconds using MQTT.
   - The same data is also stored in a local log file with timestamps.

3. **Data Retrieval (Offline)**  
   - `last_5_hour_data.py` filters the logged data to show values from the last 5 hours for a specific sensor.
   - This demonstrates the ability to perform time-based analysis on historical data.

---

## 🚀 How To Run

1. **Install dependencies**
2. **Replace MQTT credentials in** `mqtt_thingspeak_publisher.py`
3. **Run the script**  
4. **Watch the live graphs on your ThingSpeak channel dashboard**  

---

## 📸 Screenshots

Screenshots of the following were included in the submission pdf file :
- ThingSpeak Channel Dashboard with live graph updates
- MQTT Device credentials screen
- Console output from both python scripts
- Contents of the `sensor_log.txt` file

---

## ✍️ Author

**Venkata Sri Siva Ramakrishna Palaparthy**  
Syracuse University – M.S. Computer Science  

---
