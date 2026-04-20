IoT-Based Fire Detection System
Overview

This project is an IoT-based Fire Detection System designed to detect fire hazards using smoke, gas, and temperature sensors. It sends real-time alerts to users through a mobile app or web interface using Wi-Fi-enabled microcontrollers like ESP8266/ESP32.

Features
Real-time fire detection
Temperature monitoring
Smoke and gas detection
Instant alerts via mobile/web
Wi-Fi connectivity (IoT enabled)
Low cost and energy efficient
Technologies Used
Arduino / ESP8266 / ESP32
Embedded C / Arduino IDE
Blynk / Firebase / MQTT
Sensors (MQ-2, DHT11, Flame Sensor)
Components Required
ESP8266 / ESP32
MQ-2 Gas Sensor
DHT11 Temperature Sensor
Flame Sensor
Buzzer
Jumper Wires
Breadboard
Working Principle

The system continuously monitors environmental conditions using sensors. If abnormal values (high temperature, smoke, or gas) are detected:

Data is processed by the microcontroller
Alert is triggered via buzzer
Notification is sent to the user via IoT platform
Project Diagram

Start
↓
Initialize ESP8266 and Sensors
↓
Connect to Wi-Fi
↓
Connect to Blynk Cloud
↓
Read Flame Sensor Data
↓
Read Gas Sensor Data
↓
Flame or Gas Detected?
↓

Yes → Turn ON LED → Activate Buzzer → Send Alert to Blynk App → Update Monitoring → Repeat

No → Keep LED & Buzzer OFF → Repeat


License

This project is open-source and available under the MIT License.

Author
Rose Alice Ekka
