---
layout: page
title: ESP32 Smart Light
description: ESP-IDF IoT LED Controller with BLE provisioning, HTTP control, NVS storage, and OTA updates
img: assets/img/esp32_project/ESP32_banner.jpg
importance: 1
category: fun
related_publications: true
---

---

<br/>

## 💡 Project Overview

The **ESP32 Smart Light** is a custom firmware project built with the ESP-IDF framework in C.  
It’s designed to control an LED over WiFi, with **Bluetooth Low Energy (BLE)** provisioning,  
**HTTP-based control**, **non-volatile storage (NVS)** for persistent settings, and  
**over-the-air (OTA)** firmware updates for easy maintenance.

The project demonstrates my ability to connect **hardware and software**,  
from low-level embedded development to network protocols and update mechanisms.

<br/>

## ⚙️ Key Features

- **BLE WiFi Provisioning** — Configure WiFi credentials via Bluetooth from a mobile device.
- **HTTP API Control** — Control LED state using REST-style requests.
- **NVS Storage** — Save and retrieve configuration data persistently.
- **OTA Updates** — Deploy firmware updates remotely without a wired connection.
- **Built with ESP-IDF in C** — Full control over hardware features.

<br/>

## 📂 Repository

🔗 [View on GitHub]() (_coming soon_)

<br/>

## 🛠️ Hardware Setup

Below is the ESP32-C6 Mini hardware used in the project, shown both in real life and as a wiring diagram for clarity.

<div class="row justify-content-left text-center">
    <div class="col-md-5 mb-3">
        {% include figure.liquid path="assets/img/esp32_project/esp32_board_layout.jpg" 
           title="Real-life setup" class="img-fluid rounded z-depth-2" %}
        <p class="small text-muted mt-2">Real hardware on a breadboard</p>
    </div>
    <div class="col-md-5 mb-3">
        {% include figure.liquid path="assets/img/esp32_project/esp32_diagram.png" 
           title="Wiring diagram" class="img-fluid rounded z-depth-2" %}
        <p class="small text-muted mt-2">Wiring: GPIO 23 → LED → 220 Ω resistor → GND</p>
    </div>
</div>

<br/>

## 📶 BLE Device Setup

The mobile app enables BLE-based provisioning for your ESP32 Smart Light.  
You can scan for nearby ESP32 devices, connect, and send WiFi credentials from your phone.  
This process allows the device to join your local network without hardcoding credentials.

<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/mobile_app/esp32_scan_ble_devices.jpg" title="Web UI for LED control" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/mobile_app/esp32_send_wifi_credentials.jpg" title="BLE WiFi setup screen" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/hardware_logs/esp32_wifi_set_up_log.png" title="WiFi Set Up Logs" class="img-fluid rounded z-depth-1" max-width="600px" %}
    </div>
</div>
<div class="caption">
    The BLE provisioning screen scans for nearby devices and allows you to send WiFi credentials from your phone to the ESP32 device. After connection you can toggle LED and update the hardware.
</div>

<br/>

## 🏠 Home & Control Screens

Below you can see the main device list and the control interface for an individual ESP32 Smart Light.  
The home screen shows all discovered devices on your network, while the control screen allows you to toggle the light and view device details.

<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/mobile_app/esp32_home_screen_device_list.jpg" title="Home Screen" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/mobile_app/esp32_device_control_screen.jpg" title="Device Control Screen" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
</div>
<div class="caption">
    The home screen shows all discovered devices on your network, while the control screen allows you to toggle the light and view device details. The device control interface lets users toggle and update the device after a successful connection.
</div>

<div class="text-center">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/hardware_logs/esp32_light_toggle_log.png" title="Toggle Logs" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
</div>
<div class="caption">
    IDF monitor log of light toggling.
</div>

<br/>

## 🔄 OTA Update Screen

The ESP32 Smart Light supports over-the-air (OTA) firmware updates directly from the mobile app.  
The screenshot below shows the OTA update process in progress, allowing you to seamlessly upgrade your device without physical access.

<div class="row">
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/mobile_app/esp32_ota_update.jpg" title="OTA Update Screen" class="img-fluid rounded z-depth-1" max-width="350px" %}
    </div>
    <div class="col-sm mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/esp32_project/hardware_logs/esp32_ota_update_log.png" title="OTA Update Logs" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    OTA update in progress: The app downloads and installs new firmware to the ESP32 device over WiFi.
</div>

<br/>

## 📃 Summary

In short, this was my "forever project" where there is only more to develop and the expansion of the project is only limited by my own time and interest.

Next, I might add an RGB LED and frontend controller for it. Or whatever comes to mind. Motors? Scanners? Who knows! 😄

If you're interested in the source code, check here: [Repository](#-repository)

<br/>
