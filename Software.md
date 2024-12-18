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
```  

### Step 3: Upload the Code  
- Connect your ESP32 microcontroller to your computer.  
- Open the provided `.ino` file in Arduino IDE.  
- Select the correct board:  
   `Tools -> Board -> ESP32 Dev Module`  
- Select the correct port:  
   `Tools -> Port`.  
- Upload the code to your ESP32.  

### Step 4: Visualize Data  

#### On Web  
1. Log in to the [Blynk Website](https://www.blynk.io/).  
2. Create a project.  
3. Add widgets (e.g., gauges, graphs) to display sensor data.  

#### On Mobile  
1. Download the Blynk app.  
2. Log in and create your project.  
3. Add widgets for monitoring data.  

#### Locally  
- The OLED display will automatically show real-time air quality data.  

---

## Code Overview  

### Key Functionalities  

1. **Sensors Initialization:**  
   - **BME680:** Measures temperature, humidity, and gas levels.  

2. **WiFi and Blynk Setup:**  
   - Establishes a connection to the internet.  
   - Integrates with the Blynk platform.  

3. **Data Visualization:**  
   - Sends sensor data to Blynk for remote visualization.  
   - Displays data locally on the OLED screen.  

---

## Required Updates  

1. **WiFi Credentials:**  
   Update `WIFI_SSID` and `WIFI_PASSWORD` with your WiFi network's credentials.  

2. **Blynk Authentication:**  
   Replace `BLYNK_AUTH_TOKEN` with your project's authentication token from the Blynk dashboard.  

---

## Visualization  

### OLED Monitor  
- Displays real-time data directly on the device.  

### Web Interface  
- Provides detailed charts and logs through the Blynk platform.  

### Mobile Interface  
- Offers a user-friendly way to monitor data on the go via the Blynk app.  

---

## Future Enhancements  

- Add more advanced sensor calibration.  
- Support additional visualization platforms.  

---

## References  

- [Blynk Documentation](https://docs.blynk.io/)  
- [Arduino Libraries Documentation](https://www.arduino.cc/en/Reference/Libraries)
