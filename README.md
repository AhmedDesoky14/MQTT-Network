# MQTT-Network
`MQTT-Network` is Client application for MQTT communications between many IoT nodes represnted by STM32F4x micrcontrollers connected to ESP8266 WiFi modules using UART-based serial communications.
This is part of the **Secured V2X Enabled Autoparking System Graduation Project**, mentored by **Valeo**.

This application is Client side. MQTT broker used is "Mathworks Thingspeak" free MQTT broker. Also Client application for Thingspeak brokers is developed.

## Features
- Seamless communications with other MQTT clients connected to the same MQTT broker.
- Subscribing to more than 1 topic at MQTT broker.
- Publishing topics to MQTT broker.
- Handle all exchanged messages asynchronously.

---

## Components
- ESP8266 WiFi hardware module, based on STM HAL libraries.
- Paho MQTT C Packet external library for requests serialization and deserialization.
- cJSON external library for handling requests in JSON using C langauge.
- MQTT Client module. to deal in general with different types of MQTT brokers. publish topics and subscribe to topics.
- Thingspeak MQTT module. wrapper application for MQTT Client module to handle requests with Thingspeak Broker using JSON.

---

## External Dependencies
- Paho MQTT C Packet library.
- cJSON library.
- Established Broker.

---

**All communications and data exchange are handled asynchronously using:**
- Interrupts by NVIC on STM32F1x microcontrollers

**NOTE:** cryptography keys need to be configured. Examples are provided.

**Authors:**
	Ahmed Desoky,
	
**Emails:**
	ahmed0201150@gmail.com,
