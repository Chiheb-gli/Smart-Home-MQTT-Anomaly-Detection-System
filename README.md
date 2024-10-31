# Smart Home MQTT Anomaly Detection System - Initialization

This branch provides instructions to set up the development environment for the Smart Home MQTT Anomaly Detection System, including installing required tools and dependencies.

## Prerequisites

The following tools and libraries are required for this project:
- **MQTT Broker**: Mosquitto
- **Node-RED**: For simulating smart home network nodes
- **Python**: Development environment with Scapy for packet analysis and ML packages for anomaly detection

---

## Installation Guide

### 1. Install MQTT Broker - Mosquitto
Mosquitto is an open-source MQTT broker that manages message distribution in the MQTT network.

- **Windows**: Download and install from [Mosquitto's official site](https://mosquitto.org/download/).
- **Linux**: Use the following commands:
  
bash
  sudo apt update
  sudo apt install mosquitto mosquitto-clients
  sudo systemctl enable mosquitto  # Start Mosquitto on boot

- **Mac**: Use Homebrew:

- bash
mosquitto



### 2. Install Node-RED
Node-RED is used to create and manage the simulated network of smart home devices.

**Installation**:
- Windows/macOS/Linux: Run the following command:
- 
### 2. Install Node-RED
Node-RED is used to create and manage the simulated network of smart home devices.

**Installation**:
- Windows/macOS/Linux: Run the following command:
  

### 2. Install Node-RED
Node-RED is used to create and manage the simulated network of smart home devices.

**Installation**:
- Windows/macOS/Linux: Run the following command:
  
bash
  npm install -g --unsafe-perm node-red
    

**Starting Node-RED**:
bash
node-red



**Accessing Node-RED**: Once started, open [http://localhost:1880](http://localhost:1880) in a web browser to access the Node-RED interface.

### 3. Set Up Python Environment
Python 3.7+ is required for this project.

**Step 1**: Create a Virtual Environment (recommended to isolate dependencies):

bash
python -m venv env
source env/bin/activate   # Linux/macOS
.\env\Scripts\activate    # Windows



**Step 2**: Install Required Packages: Create a requirements.txt file with the following packages:

scapy         # For packet capturing and analysis
paho-mqtt     # MQTT client library in Python
numpy         # Numerical computing library for ML
scikit-learn  # ML library with models for anomaly detection


Install packages from requirements.txt:

bash
pip install -r requirements.txt


### 4. Install Scapy and ML Packages
**Scapy**: Scapy is used to capture and inspect MQTT traffic at the packet level.

bash
pip install scapy




**ML Packages for Anomaly Detection**:

- **NumPy**: Provides efficient data structures and mathematical operations.
- **Scikit-learn**: For ML models like Isolation Forest, useful for unsupervised anomaly detection.

Install these with:



**ML Packages for Anomaly Detection**:

- **NumPy**: Provides efficient data structures and mathematical operations.
- **Scikit-learn**: For ML models like Isolation Forest, useful for unsupervised anomaly detection.

Install these with:

bash
pip install numpy scikit-learn




## Next Steps
Once all tools are installed:

1. **Set up the Node-RED flow**: Configure simulated devices to publish MQTT data.
2. **Run the Python script**: Use Python to capture MQTT packets and feed them to the ML model.
3. **Train and Test the ML Model**: Train an unsupervised model to identify anomalies in smart home device data.

This setup completes the initial environment configuration for the project. Check back on the main branch for more advanced setup and usage details.










  

  
