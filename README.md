🚦 Dynamic Traffic Management Using Real-Time Density Estimation

An Arduino UNO R4 WiFi-based smart traffic management system that dynamically controls traffic signals using real-time vehicle density. The system uses six IR sensors to monitor traffic across three roads, calculates congestion levels, and allocates adaptive green signal timings to reduce waiting time and improve traffic flow.

---

📌 Overview

Traditional traffic signals operate on fixed timers, leading to unnecessary delays and congestion. This project introduces a density-based traffic control system that adapts signal timings according to real-time traffic conditions, improving intersection efficiency and reducing fuel consumption.

---

✨ Features

- 🚗 Real-time vehicle density detection
- 🚦 Adaptive traffic signal timing
- 📊 Congestion-based lane prioritization
- ⏱️ Queue length and waiting time monitoring
- 📟 Live traffic status on a 16×2 I2C LCD
- 🔄 Continuous traffic re-evaluation

---

🛠 Hardware Components

- Arduino UNO R4 WiFi
- 6 × IR Sensors
- 16×2 I2C LCD
- 9 × LEDs (Red, Yellow, Green)
- Breadboard
- Jumper Wires
- USB Cable

---

⚙️ Working Principle

Each of the three roads is equipped with two IR sensors:

- **S1 (Near Sensor):** Detects the queue length near the traffic signal.
- **S2 (Far Sensor):** Detects approaching vehicles and estimates the arrival rate.

The Arduino continuously evaluates:

- Queue Length
- Vehicle Arrival Rate
- Waiting Time
- Congestion Level

The lane with the highest congestion is assigned the green signal for an adaptive duration. After each cycle, the traffic conditions are recalculated to determine the next priority.

---

📂 Project Structure

```text
Arduino_Code/
Circuit_Diagram/
Documentation/
Images/
Videos/
README.md
LICENSE
```

---

🚀 Getting Started
🚀 Getting Started

1. Clone this repository.
2. Open the Arduino sketch in the Arduino IDE.
3. Connect the hardware according to the circuit diagram.
4. Upload the code to the Arduino UNO R4 WiFi.
5. Power the system and observe adaptive traffic signal control.

---

📸 Project Images

Add your project images here.

Example:

```
Images/
├── Prototype.jpg
├── Circuit_Diagram.png
├── LCD_Output.jpg
```

---

🔮 Future Enhancements

- IoT-based remote traffic monitoring
- Emergency vehicle priority detection
- Camera-based vehicle counting
- AI/ML-based traffic prediction
- Cloud dashboard for live traffic analytics

---

👨‍💻 Author

**Nishit Gupta**

---

📄 License

This project is licensed under the MIT License.
