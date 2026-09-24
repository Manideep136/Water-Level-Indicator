# Water-Level-Indicator
Project Overview

This project is an ESP32-based Water Level Indicator PCB designed to monitor the water level in a tank using an ultrasonic sensor and provide visual and audible alerts.

The PCB is designed in KiCad and provides connections for an ESP32 DevKit V1 (30-pin), ultrasonic sensor, OLED display, buzzer, LED indicator, push button, and power supply.

The ESP32 processes the distance measured by the ultrasonic sensor and determines the approximate water level. The status can be displayed on an OLED and indicated using LEDs and a buzzer.

Features
ESP32 DevKit V1 based controller
Ultrasonic water-level measurement
OLED display interface using I²C
LED status indication
Buzzer alarm for high/critical water level
Push-button input
Transistor-driven buzzer circuit
Removable ESP32 module
Through-hole mounting for ESP32 headers
External 5 V DC power input
Designed using KiCad
PCB layout suitable for prototype/college project development



🚀 Working Principle
The ultrasonic sensor sends an ultrasonic pulse toward the water surface.
The reflected signal is received by the sensor.
The ESP32 calculates the distance to the water surface.
The water level is calculated from the tank dimensions.
The current water-level status can be displayed on the OLED.
LEDs provide visual status indication.
The buzzer provides an audible warning when the water reaches a defined critical level.
The push button provides an additional user-control interface.
🔧 Future Improvements

Possible future versions can include:

Automatic water pump control
Wi-Fi monitoring
Mobile/web dashboard
MQTT/ThingsBoard integration
Water-level percentage calculation
Multiple tank monitoring
Low-water warning
Overflow protection
Relay/SSR output
Capacitive water-level sensing
PCB-mounted voltage regulator and protection circuit
⚠️ Important Design Notes
Verify the exact ESP32 DevKit V1 dimensions before PCB manufacturing.
Verify the 25.40 mm header row spacing against the physical ESP32 board.
Use 2.54 mm pitch headers.
Use appropriate voltage-level protection for a 5 V ultrasonic ECHO signal.
Keep sensor wiring away from noisy/high-current traces.
Use an external certified DC power supply for the prototype.
Check ERC and DRC before generating Gerber files.
Verify all connector pinouts before manufacturing.
📜 License

This project is intended for educational, academic, and personal development purposes.

Feel free to modify and improve the design for your own projects.
