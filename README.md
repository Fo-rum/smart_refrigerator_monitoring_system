# 🧊 Smart Refrigerator Monitoring System

## Project Overview

This project implements a **Smart Refrigerator Monitoring System** that tracks temperature, humidity, and inventory data using IoT sensors and transmits it to a server for monitoring. Built using the ESP32 (or ESP8266) and PlatformIO, the system provides alerts for restocking and environmental anomalies like temperature spikes or humidity drops.

It includes a Python-based backend to log or analyze incoming sensor data, making this a complete edge-to-cloud IoT solution.

---

## Features

- ✅ Real-time monitoring of temperature and humidity
- ✅ Inventory tracking using weight sensors or RFID tags
- ✅ Automatic data upload to a server via Wi-Fi
- ✅ Alert generation for restocking and abnormal conditions
- ✅ Modular, expandable system structure

---

## Files Included

| File/Folder | Description |
|-------------|-------------|
| `src/main.cpp` | Core firmware code for the ESP32 device. |
| `server.py` | Python backend server to receive and log sensor data. |
| `platformio.ini` | PlatformIO configuration for firmware build and upload. |
| `lib/`, `include/`, `test/` | Standard PlatformIO directories for libraries, headers, and testing. |
| `.vscode/extensions.json` | Recommended VS Code extensions. |

---

## Getting Started

### Prerequisites

- **PlatformIO** with VS Code or CLI
- **Python 3.6+** for running `server.py`
- ESP32 or ESP8266 microcontroller
- Sensors (e.g., DHT22, HX711 for weight sensing)

### Firmware Setup

1. Open the project folder with [PlatformIO](https://platformio.org/)
2. Connect your ESP32/ESP8266 device.
3. Upload the code using:

```bash
pio run --target upload
```

Or click the "Upload" button in the PlatformIO interface.

### Backend Setup

1. Install Python dependencies (if any):

```bash
pip install -r requirements.txt
```

2. Run the server:

```bash
python server.py
```

---

## Project Structure

```
├── src/main.cpp
├── server.py
├── platformio.ini
├── lib/
├── include/
├── test/
└── .vscode/
```

---

## Technologies Used

- **C++** with PlatformIO for firmware development
- **Python 3** for the backend server
- **ESP32/ESP8266** as IoT hardware
- **Wi-Fi**, **DHT22**, **HX711** or RFID for sensing

---

## Notes

- Make sure the microcontroller is connected before uploading firmware.
- The server script can be modified to log data to a database or cloud platform.
- This project is ideal for smart home automation, food safety, and inventory control.
