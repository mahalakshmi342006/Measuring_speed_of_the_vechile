# 🚗 Measuring Speed of Vehicle Using Arduino

An Arduino-based vehicle speed measurement system that calculates the speed of a moving vehicle using two IR sensors placed at a fixed distance. The measured speed is displayed on an LCD, and a buzzer provides an alert when the speed exceeds a predefined limit.

## 📌 About the Project

Road safety is an important concern, and overspeeding is one of the factors that can contribute to accidents. This mini project demonstrates a simple and cost-effective method of measuring vehicle speed using embedded systems.

The system detects a vehicle passing two IR sensors, calculates the time taken to travel between them, and determines the speed using the formula:

**Speed = Distance / Time**

The result is displayed on an LCD, and an alert is generated when the measured speed exceeds the set speed limit.

## ✨ Features

* 🚗 Vehicle movement detection
* ⏱️ Time measurement between two fixed points
* 📏 Speed calculation
* 📺 Real-time LCD display
* 🔔 Overspeeding alert using a buzzer
* 🔧 Simple and low-cost embedded system

## 🛠️ Components Used

| Component         | Purpose                                     |
| ----------------- | ------------------------------------------- |
| Arduino UNO       | Processes sensor data and calculates speed  |
| IR Sensors ×2     | Detect vehicle movement at two fixed points |
| 16×2 LCD with I2C | Displays the measured speed                 |
| Buzzer            | Alerts when the speed exceeds the limit     |
| Breadboard        | Circuit prototyping                         |
| Jumper Wires      | Component connections                       |

## ⚙️ Working Principle

1. Two IR sensors are placed at a known fixed distance.

2. When a vehicle crosses the first sensor, the starting time is recorded.

3. When the vehicle crosses the second sensor, the ending time is recorded.

4. The Arduino calculates the time difference.

5. Speed is calculated using:

   **Speed = Distance / Time**

6. The measured speed is displayed on the LCD.

7. If the speed exceeds the predefined limit, the buzzer is activated.

## 📐 Speed Calculation

```text
Speed = Distance / Time
```

For example, if the distance between the sensors is **20 cm** and the vehicle takes **2 seconds**:

```text
Speed = 20 / 2
      = 10 cm/s
```

The distance and time values can be adjusted according to the actual experimental setup.

## 🔌 System Flow

```text
Vehicle Movement
       ↓
IR Sensor 1 Detects Vehicle
       ↓
Record Starting Time
       ↓
IR Sensor 2 Detects Vehicle
       ↓
Record Ending Time
       ↓
Calculate Time Difference
       ↓
Calculate Vehicle Speed
       ↓
Display Speed on LCD
       ↓
Compare with Speed Limit
       ↓
Overspeed? ── Yes ──→ Buzzer Alert
       │
       No
       ↓
Continue Monitoring
```

## 🚀 How to Run

1. Install the Arduino IDE.
2. Connect the Arduino UNO to your computer.
3. Connect the IR sensors, LCD, and buzzer according to the circuit diagram.
4. Open the Arduino source code.
5. Select **Arduino UNO** as the board.
6. Select the correct COM port.
7. Upload the code.
8. Place the IR sensors at a fixed distance.
9. Test the system using a moving vehicle or model car.

## 📂 Project Structure

```text
vehicle-speed-measurement-arduino/
│
├── README.md
├── code/
│   └── vehicle_speed_measurement.ino
├── circuit/
│   └── circuit_diagram.png
├── images/
│   └── project_setup.jpg
└── report/
    └── mini_project_report.pdf
```

## 🎯 Applications

* Traffic speed monitoring
* School-zone safety systems
* Residential road monitoring
* Embedded systems learning
* Accident prevention demonstrations

## 🔮 Future Improvements

* Add wireless monitoring using ESP32
* Store speed data for analysis
* Add a camera-based vehicle detection system
* Improve measurement accuracy
* Add a web dashboard for real-time monitoring

**Department of Electronics and Communication Engineering**
**St. Joseph's Institute of Technology**

## 📄 Project Report

The complete mini project report is included in the `report/` folder.

---

⭐ If you find this project useful, consider giving the repository a star!

