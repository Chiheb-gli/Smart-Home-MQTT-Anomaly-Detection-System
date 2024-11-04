# Smart Home MQTT Anomaly Detection System - Initialization

This branch provides instructions to set up the development environment for the Smart Home MQTT Anomaly Detection System, including installing required tools and dependencies.

## Prerequisites

The following tools and libraries are required for this project:

- **MQTT Broker**: Mosquitto
- **Node-RED**: For simulating smart home network nodes
- **Python**: Development environment with Scapy for packet analysis and ML packages for anomaly detection

## Installation Guide

### 1. Install MQTT Broker - Mosquitto

Mosquitto is an open-source MQTT broker that manages message distribution in the MQTT network.

- **Windows**: Download and install from [Mosquitto's official site](https://mosquitto.org/download/).
- **Linux**: Use the following commands:

- bash
- sudo apt update
- sudo apt install mosquitto mosquitto-clients
- sudo systemctl enable mosquitto # Start Mosquitto on boot
