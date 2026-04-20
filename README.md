Fire Detection System using NodeMCU and Blynk
Overview
This project is an IoT-based Fire Detection System built using NodeMCU (ESP8266) and the Blynk app. It detects fire using a flame sensor and gas sensor, and sends real-time alerts to the user.

When fire or gas leakage is detected:

LED turns ON
Buzzer sounds
Notification is sent via Blynk app
Components Required
NodeMCU (ESP8266)
Flame Sensor
Gas Sensor (MQ series)
LED
Buzzer
Jumper Wires
Breadboard
Pin Configuration
Component	NodeMCU Pin
Flame Sensor	D2
Gas Sensor	A0
LED	D7
Buzzer	D5
Blynk Setup
Create a project in Blynk IoT

Add widgets:

V0 → LED Indicator (Fire Status)
V1 → Value Display (Gas Sensor)
Create an event named: fire_alert

Add your Template ID and Auth Token in the code

Code Explanation
flamePin: Detects fire (LOW = fire detected)
gasPin: Reads gas value using analog input
Blynk.virtualWrite(V1, gasValue): Sends gas data to the app
Blynk.logEvent(): Sends alert notification
Detection Logic
if (flame == LOW || gasValue > 400)
If flame is detected or gas value crosses the threshold, the system triggers an alert.

Features
Real-time monitoring using Blynk
Instant mobile notifications
Dual detection using flame and gas sensors
Simple and low-cost solution
Working
The system continuously reads sensor values

If fire or gas is detected:

LED turns ON
Buzzer turns ON
Alert is sent to the mobile app
Otherwise, the system stays in normal state

Future Improvements
Add temperature sensor (DHT11 or DHT22)
Add SMS alert using GSM module
Integrate automatic fire suppression system
Improve threshold calibration
Author
Rose Alice Ekka

License
This project is open-source and free for educational use.
