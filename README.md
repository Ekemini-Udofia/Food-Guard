## Overview

This project is a smart pantry and food storage monitoring system designed to detect early-stage food spoilage and mold risks. Built on the ESP32-S3 SuperMini, the device measures ambient temperature and pressure using a BMP280 sensor, humidity via a DHT11 module, and off-gassing volatile organic compounds using an MQ-135 sensor.

## Key Features

- Dual Climate & Gas Sensing: Combines multi-sensor inputs to run local Dew Point calculations and detect chemical decay off-gassing.
- Hardware Power-Gating: Utilizes an N-channel logic-level MOSFET (IRLB8721) to power-gate the 5V boost converter and MQ-135 heater during sleep cycles, significantly reducing battery consumption.
- Low-Power IoT Architecture: Employs ESP32 deep sleep to maximize battery runtime on a single 3.7V LiPo cell while pushing periodic updates over Wi-Fi.