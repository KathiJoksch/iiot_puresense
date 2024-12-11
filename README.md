# Pure Sense (IIoT)
PureSense brings you a portable solution to monitor indoor air quality. With a compact design, our device offers real-time data, allowing you to understand and manage the air you breathe. PureSense is created to be user-friendly, accessible, and effective in maintaining safe and healthy indoor environments.

## About us
We are a group of 5 people, who develop an air quality monitoring tool during our IIoT course at Taiwan Tech (National Taiwan University of Science).

## Hardware

### Components
Our air quality monitoring solution is built using the following hardware components:
- __Firebeetle ESP32-E Microcontroller__
A powerful and energy-efficient microcontroller featuring a dual-core processor, built-in Wi-Fi, and Bluetooth. It ensures smooth data processing and connectivity for our device. [Link to Product](https://bit.ly/2VYygmj)

- __Gravity Analog Infrared CO2 Sensor__
The Gravity Analog Infrared CO2 Sensor accurately measures carbon dioxide (CO₂) levels in the air. It operates using infrared light to detect CO₂ absorption, one of the most reliable methods for gas measurement. This makes it an excellent choice for monitoring indoor air quality and ensuring a safe environment. [Link to Product](https://amzn.to/3CrzOGm)

- __BME280 Environment Sensor__
The BME280 environment sensor is designed to measure temperature, humidity, and air pressure with high precision. It utilizes advanced MEMS (Micro-Electro-Mechanical Systems) technology, enabling reliable multi-environment sensing. This makes it ideal for detecting changes in indoor climate conditions and maintaining optimal comfort levels. [Link to Product](https://amzn.to/3sVXmQw)

- __I2C OLED Display__
A compact display module that provides a clear and efficient interface for real-time data visualization. [Link to Product](https://amzn.to/3MFgTg7)

- __Set of Various Screws & M3 Brass Inserts__
Essential hardware for securely assembling the device. [Link to Product](https://amzn.to/3J2Bskq) & [Product Link](https://amzn.to/3MBvEjS)

- __2mm Clear Acrylic__
A durable, transparent material used for the device casing, ensuring visibility and protection. [Link to Product](https://amzn.to/3vRgL7d)

### Architecture
The architecture of PureSense is designed to provide a seamless integration of hardware components, ensuring reliability and portability. At its core lies the Firebeetle ESP32-E Microcontroller, which serves as the central processing unit, managing data collection, processing, and communication. Environmental data is continuously gathered by the BME280 Environment Sensor, which measures temperature, humidity, and air pressure, and the Gravity Analog Infrared CO2 Sensor, which monitors carbon dioxide levels. This information is then processed by the ESP32 and displayed in real-time on the I2C OLED Display, allowing users to instantly assess air quality.

Wireless connectivity is a key feature of the architecture, enabled by the ESP32's built-in Wi-Fi module. This allows the device to transmit data to external platforms for remote monitoring, creating opportunities for cloud-based analytics and broader integrations. The hardware assembly is compact and robust, constructed with a transparent 2mm acrylic casing that ensures both visibility and protection of the internal components. Secured with M3 brass inserts and screws, the design is both durable and easy to maintain, making PureSense ideal for portable use.

## Software
The software of PureSense is developed to maximize functionality while maintaining user-friendliness and efficiency. The ESP32 microcontroller is programmed using the Arduino IDE, which provides a flexible platform for integrating the various sensors and components. Custom code retrieves data from the BME280 and Gravity CO2 sensors, processing it to display temperature, humidity, air pressure, and CO2 levels accurately.

Real-time data is dynamically presented on the OLED display, giving users immediate insights into the air quality of their environment. Additionally, the software is designed to support optional cloud integration, enabling remote data storage and monitoring for more comprehensive air quality management. Power efficiency is a critical feature of the system, with the ESP32 optimized for low-power operation to extend battery life and ensure sustained performance.

This combination of advanced hardware and thoughtfully developed software ensures that PureSense is not only effective in monitoring indoor air quality but also scalable and adaptable for a variety of applications.

