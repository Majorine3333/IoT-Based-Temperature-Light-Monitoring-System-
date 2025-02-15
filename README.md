# PROJECT OVERVIEW
This project involves the development of a Smart Environmental Monitoring System that tracks temperature, humidity, and light intensity in at least two different locations (indoors and outdoors). The system is designed to collect, display, and store data while offering flexible data submission methods and remote configuration options.
**Features**
Real-time monitoring of:
- Temperature (every 6 seconds)
- Humidity (every 3 seconds)
- Light intensity (every 6 seconds)

**Data Posting Methods:**
- HTTP POST to a database
- MQTT publishing to a broker

**Database Design**: Supports multiple smart nodes dynamically without modification.

**Web Interface on a Web Server**:
- View historical sensor data.
- Add new smart nodes and assign descriptive names.
- View data submitted by any specific smart node.
**Smart Object Features:**
- LCD displays real-time sensor values and device IP.
- Built-in web portal for direct interaction (via phone or PC).
- Allows switching between HTTP POST and MQTT.
- Supports over-the-air (OTA) updates.
- Controls an AC-powered fan(relay), either manually or automatically based on a temperature threshold.


# INSTALLATION AND SETUP
**Prerequisites**
**Hardware**: ESP32/ESP8266 with sensors (DHT11/DHT22 for temperature & humidity, LDR for light intensity)
**Software**:
Python 3
PHP & MySQL (for web server and database)
MQTT Broker (e.g., Mosquitto)
Arduino IDE (for smart object programming)

**Steps to Run the Project**

Set up the database using the provided schema.

Deploy the web server (Apache with PHP & MySQL recommended).

Run the MQTT broker (Mosquitto or any cloud-based broker).

Flash the ESP32 with the firmware (found in finalproject_IOT_arduino).

Execute mqttscript_final.py to test MQTT connectivity.

Access the web portal to view and configure the system.
