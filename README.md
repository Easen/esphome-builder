# My ESPHome Builder

This repository provides a simple Docker Compose configuration for running [ESPHome](https://esphome.io/)—an open-source system for managing ESP8266/ESP32 smart devices using YAML configuration files.

## Features
- Easy deployment with Docker Compose
- Persistent configuration storage in `config/`
- ESPHome dashboard available at [http://localhost:6052](http://localhost:6052)

## Project Structure
- `config/` — Stores ESPHome YAML configuration files and device data
- `docker-compose.yml` — Main Docker Compose configuration

## Getting Started

### Prerequisites
- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Setup & Usage
1. Start ESPHome:
   ```sh
   docker compose up
   ```
2. Open your browser and go to [http://localhost:6052](http://localhost:6052)
3. Profit!

### Configuration
- All configuration and device data are persisted in `config/`.


## References
- [ESPHome Documentation](https://esphome.io/)
- [Docker Compose Documentation](https://docs.docker.com/compose/)

---

## ESPHome Configurations

This repository includes my ESPHome YAML configuration files in the `config/` directory:

- **esp32-bluetooth-proxy-1.yaml** and **esp32-bluetooth-proxy-2.yaml**
   - Configure ESP32 devices as Bluetooth proxies for Home Assistant.
   - Use the official ESPHome Bluetooth Proxy package from GitHub.
   - WiFi credentials and API encryption keys are referenced from secrets.
   - Each file sets a unique device name and friendly name for easy identification.

- **konnected-e2481d.yaml**
   - Example configuration for a Konnected Alarm Panel (ESP8266-based).
   - Uses remote packages from the Konnected ESPhome repository for modular setup.
   - Defines switches and binary sensors for alarm zones and siren control.
   - Includes advanced options like status LED, warning beep, and verbose logging.
   - WiFi credentials and API encryption keys are referenced from secrets.

---
Contributions and suggestions are welcome!
