# Air Quality Monitoring System
*By Salma*

This repository contains the software component for an Air Quality Monitoring System. The software is designed to interface with an ESP32 microcontroller and other sensors to monitor air quality, providing real-time data visualization locally on an OLED screen and remotely via the Blynk platform.  

---

## Features  

### Local Monitoring  
- Displays real-time environmental data (e.g., temperature, humidity, CO₂ levels) on an OLED screen.  

### Remote Monitoring  
- Integrates with the Blynk platform for data visualization on both web and mobile applications.  

### Configurable Settings  
- Easily update WiFi and Blynk authentication credentials in the code.  

---

## Requirements  

### Hardware  
- **ESP32 microcontroller**  
- **Adafruit BME680 sensor** (for temperature, humidity, and gas measurements)  
- **OLED display** (128x64 resolution)  

### Software  
- **Arduino IDE**  

#### Required Libraries  
- `Esp32WifiManager`  
- `Adafruit_BME680`  
- `Adafruit_SSD1306`  
- `BlynkSimpleEsp32`  

---

## Blynk Integration  

### Web-based Visualization  
- [Blynk Website](https://www.blynk.io/)  

### Mobile-based Visualization  
- Download the Blynk app from the [App Store](https://apps.apple.com/) or [Google Play](https://play.google.com/).  

---

## Setup Instructions  

### Step 1: Install Required Libraries  
Ensure you have installed all necessary libraries in your Arduino IDE. Use the Library Manager:  
`Tools -> Manage Libraries`  
Search for and install the libraries listed in the **Requirements** section.  

### Step 2: Update WiFi and Blynk Credentials  
Replace the placeholders in the code with your actual credentials:  
```cpp
#define WIFI_SSID "Your WiFi SSID"
#define WIFI_PASSWORD "Your WiFi Password"
#define BLYNK_AUTH_TOKEN "Your Blynk Auth Token"
#define BLYNK_TEMPLATE_ID "Your BLYNK_TEMPLATE_ID"
