# IoT-Based Room Temperature & Humidity Monitoring using WEMOS D1 R1

## 📌 Project Description
This project is an Internet of Things (IoT) system designed to monitor room temperature and humidity in real-time. The main component used is the WEMOS D1 R1 microcontroller (based on the ESP8266) which is integrated with a DHT11 temperature and humidity sensor. The system operates on a Cloud-based operating system, allowing users to easily access and manage monitoring reports. By utilizing this tool, users can prevent property damage and health hazards caused by improper room temperature and humidity conditions.

## 🎯 Goals and Benefits
*   **Real-time Monitoring:** Accurately monitors room temperature and humidity in real-time and displays the information through a mobile and web application.
*   **Easy Access:** Transmits high-precision monitoring data directly to users via an IoT network.
*   **Automation Potential:** The Wemos D1 R1 can also be configured to control fans, air conditioners (AC), or heating systems, allowing users to wirelessly control and adjust room environments remotely.

## 🛠️ Hardware Requirements
1. Wemos D1 R1 (Equipped with 16MB onboard memory to handle heavy IoT communication tasks)
2. DHT11 Sensor
3. Jumper Wires
4. Micro USB Cable

## 🔌 Wiring Diagram

<img width="1400" height="844" alt="gambar" src="https://github.com/user-attachments/assets/7f899fa1-60fa-4756-88f0-27aa3994556a" />

*Figure: Fritzing wiring scheme showing the pin connections between the Wemos D1 R1 and the DHT11 sensor.*

The DHT11 sensor has 3 pins (VCC, GND, and DATA). The connections to the Wemos D1 R1 are as follows:
*   **VCC Pin** connects to the **5V Pin** on the Wemos.
*   **GND Pin** connects to the **GND Pin** on the Wemos.
*   **DATA Pin** connects to the **D6 Pin** on the Wemos.

## ⚙️ How It Works (System Flowchart)

<img width="306" height="870" alt="gambar" src="https://github.com/user-attachments/assets/aeca146e-3ced-4218-8cbc-91c24a18a923" />

*Figure: System workflow from device authentication to displaying real-time data on the Blynk server.*

1. The Wemos D1 R1 device authenticates and connects to the internet network.
2. The Wemos reads data from the DHT11 sensor.
3. The collected sensor data is sent to the Blynk web server.
4. The Blynk platform displays the sensor readings in real-time in the form of charts and gauges.

## 📱 User Interface (Dashboard)

**Blynk Web Dashboard:**
<img width="2130" height="984" alt="gambar" src="https://github.com/user-attachments/assets/8ceaf1aa-8011-4dea-a581-4856cded384c" />

*Figure: Real-time temperature and humidity monitoring interface on the Blynk Web Dashboard.*

**Blynk Mobile App:**
<img width="2700" height="988" alt="gambar" src="https://github.com/user-attachments/assets/014822dd-652e-48d9-b84d-6eafe14a2406" />

*Figure: Real-time temperature and humidity monitoring interface on the Blynk Mobile App.*

## 💻 Software & Libraries Used
*   Arduino IDE
*   Blynk Platform (Blynk Cloud)
*   Libraries: `ESP8266WiFi.h`, `BlynkSimpleEsp8266.h`, `DHT.h`

## License
[MIT License](LICENSE)
