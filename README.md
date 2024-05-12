# Smart Logistics

## Overview
This project focuses on developing a smart logistics system for monitoring cargo in a truck. It utilizes various sensors connected to an ESP32 microcontroller to collect data such as obstacle detection, temperature inside the cargo, engine health, and door lock status. The collected data is transmitted to a Node-RED server via MQTT protocol for further processing and storage in a MongoDB database.

## Features
- Utilizes ultrasonic sensor for obstacle detection
- Uses DHT11 sensor for temperature detection of cargo
- Integrates sound sensor for monitoring engine health
- Utilizes reed switch sensor for monitoring door lock status
- Implements MQTT communication protocol for data transmission
- Stores sensor data in a MongoDB database using Node-RED server

## Components
- ESP32 microcontroller
- Ultrasonic sensor
- DHT11 temperature and humidity sensor
- Sound sensor
- Reed switch sensor
- Raspberry Pi running Node-RED server and MongoDB database
- MQTT broker (Mosquitto) installed on Raspberry Pi

## Usage
1. Connect the sensors to the ESP32 microcontroller.
2. Configure the ESP32 with appropriate Wi-Fi credentials and MQTT broker details.
3. Deploy the Node-RED server on the Raspberry Pi and configure it to subscribe to MQTT topics for receiving sensor data.
4. Ensure that the MongoDB database is set up on the Raspberry Pi to store the received sensor data.
5. Run the ESP32 code to start collecting and transmitting sensor data.
6. Monitor and analyze the sensor data using the Node-RED dashboard.
