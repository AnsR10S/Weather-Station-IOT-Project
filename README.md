# 🌤️ Weather Station - Monitor Temperature, Humidity, Wind Speed, Rain, and Other Weather Conditions

---

## ℹ️ About the Project

This project implements a weather station using the **Arduino Uno** and various sensors to monitor environmental conditions such as temperature, humidity, pressure, and light intensity. It utilizes **Blynk** for real-time data visualization and remote monitoring. Additionally, simulated sensors for wind and rain are controlled using potentiometers. The project is developed and tested using **PicsimLab**.

## ⚙️ Features

- 🌡️ **Temperature Monitoring** (DHT11 and BMP180 Sensors)
- 💧 **Humidity Monitoring** (DHT11 Sensor)
- 🌬️ **Pressure Monitoring** (BMP180 Sensor)
- 💡 **Light Intensity Monitoring** (LDR Sensor)
- 🌬️💦 **Wind and Rain Emulation** (Potentiometers)
- 📱 **Real-Time Data Visualization** via **Blynk**
- 🌐 **Remote Monitoring** using **Ethernet W5500 Module**

## ⚙️ Working Project
![Devices-Blynk Console-GoogleChrome2024-12-2900-50-26-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/2a36f93a-b043-4b20-826a-9ce3432b43d4)
![PICSimLab-Spareparts2024-12-2900-50-01-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/7380b472-afb1-4bf6-ae51-af6be4a4e1ba)


---

## 🛠️ Components Used

1. **Arduino Uno (ATmega328P)**
2. **DHT11 Sensor** (Temperature and Humidity)
3. **BMP180 Sensor** (Temperature and Pressure)
4. **W5500 Ethernet Module** (For Internet Connectivity)
5. **LDR Sensor** (Light Intensity)
6. **Potentiometers** (Simulated Wind and Rain Sensors)
7. **LCD Display** (Optional for Local Data Display)
8. **Blynk App** (For Remote Monitoring)

Here's the updated pin connection table formatted to match the pinout descriptions you provided:

---

## 📌 Pin Connections

### 1) **BMP180 (Temperature and Pressure Sensor)**

| **Pin**   | **Connection**                           | **Description**                                          |
|-----------|------------------------------------------|----------------------------------------------------------|
| **GND**   | Ground                                   | Ground connection for the sensor.                        |
| **VCC**   | 3.3V                                     | Power supply (1.8V to 3.6V, typically 3.3V).              |
| **SCL**   | PC4/A4 (Pin 27)                          | Serial clock line for I2C communication.                 |
| **SDA**   | PC5/A5 (Pin 28)                          | Serial data line for I2C communication.                  |

### 2) **DHT11 (Humidity and Temperature Sensor)**

| **Pin**   | **Connection**                           | **Description**                                          |
|-----------|------------------------------------------|----------------------------------------------------------|
| **VCC**   | 5V                                       | Power supply (3V to 5V).                                 |
| **GND**   | Ground                                   | Ground connection.                                       |
| **DATA**  | PD2 (Pin 4)                              | Digital data output (connected to data pin of microcontroller). |

### 3) **Potentiometer (Simulating Wind and Rain Sensors)**

| **Pin**     | **Connection**    | **Description**                                              |
|-------------|-------------------|--------------------------------------------------------------|
| **VCC**     | 5V                | Power supply for the potentiometer.                          |
| **GND**     | Ground            | Ground connection.                                           |
| **Wiper/Output** | A1, A2 (Analog Inputs) | Adjustable output (simulating wind and rain conditions).   |

### 4) **Ethernet W5500 (Networking Module)**

| **Pin**   | **Connection**  | **Description**                                          |
|-----------|-----------------|----------------------------------------------------------|
| **VCC**   | 3.3V/5V         | Power supply for the Ethernet module (3.3V or 5V).       |
| **GND**   | Ground          | Ground connection.                                       |
| **SCK**   | Pin 13          | SPI Clock pin for communication.                         |
| **MISO**  | Pin 12          | Master In Slave Out (MISO) pin for SPI communication.    |
| **MOSI**  | Pin 11          | Master Out Slave In (MOSI) pin for SPI communication.    |
| **CS**    | Pin 10          | Chip Select for SPI communication.                       |
| **INT**   | Pin 2           | Interrupt pin (optional, used for triggering events).    |

---

## ▶️ How to Run the Project

1. **Setup the Arduino IDE**:
   - Install necessary libraries:
     - `DHT.h`
     - `Adafruit_BMP085_U.h`
     - `BlynkSimpleEthernet.h`
     - `SPI.h`
     - `Wire.h`

2. **Upload Code to Arduino**:
   - Connect the Arduino Uno to your PC.
   - Compile and upload the code using Arduino IDE.

3. **Configure Blynk**:
   - Install the **Blynk app** on your smartphone.
   - Use the **Blynk authentication token** provided in the code.

4. **Run Simulation in PicsimLab**:
   - Load the project into PicsimLab.
   - Connect the virtual sensors according to the pin connections.

5. **Monitor Data**:
   - View real-time data in the **Serial Monitor** and the **Blynk app**.

---

## 📊 Project Diagrams

### 1. **PicsimLab Connection Screenshot**

![image](https://github.com/user-attachments/assets/a2b1eecf-cfba-4f76-aa65-775215d82b70)

### 2. **Working Code Output**

![image](https://github.com/user-attachments/assets/9631a02b-31fe-4ca6-8b4b-46fe1c5095b0)
![image](https://github.com/user-attachments/assets/77587953-ffef-440d-8990-fc4852bbfaec)

### 3. **Sequence Diagram**

![image](https://github.com/user-attachments/assets/5171aa2f-6fc8-4d12-b188-7d745412cae5)

### 4. **Flowchart**

![image](https://github.com/user-attachments/assets/3629035a-cc23-4c9d-bc10-4cf491e01046)

---

## 🚀 Future Improvements

- **Add More Sensors** (e.g., wind speed, rainfall gauge).
- **Enhance the UI** in the Blynk app for more visualization options.
- **Implement Data Logging** to track historical weather data.
- **Add Alerts/Notifications** based on sensor thresholds.

---

## 🙏 Acknowledgments

Special thanks to:

- **Dr. Ehab Awad** for their guidance and support throughout the project.
- **TA. Hussein Mostafa** for their valuable feedback and assistance.

---

## 🌐 Further Acknowledgments

- **Blynk** for IoT platform services.
- **Adafruit** for sensor libraries.
- **PicsimLab** for simulation support.
