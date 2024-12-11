# Pure Sense (IIoT)
PureSense brings you a portable solution to monitor indoor air quality. With a compact design, our device offers real-time data, allowing you to understand and manage the air you breathe. PureSense is created to be user-friendly, accessible, and effective in maintaining safe and healthy indoor environments.

## About us
We are a group of 5 people, who develop an air quality monitoring tool during our IIoT course at Taiwan Tech (National Taiwan University of Science).

## Hardware

### Components
Our air quality monitoring solution is built using the following hardware components:
- __MH-Z14A CO2 Sensor__
The MH-Z14A CO2 sensor provides accurate carbon dioxide (CO₂) measurement with a range of 0-5000 ppm. It supports both UART and PWM output, making it highly versatile and reliable for monitoring indoor air quality.

- __Firebeetle ESP32-E Microcontroller (ESP-WROOM-32E)__
This powerful and energy-efficient microcontroller features a dual-core processor, built-in Wi-Fi, and Bluetooth. It ensures seamless data processing and connectivity for our device.

- __BME680 Environmental Sensor__
The BME680 by Bosch Sensortec is a multifunctional sensor capable of measuring temperature, humidity, air pressure, and volatile organic compounds (VOCs). Utilizing advanced MEMS (Micro-Electro-Mechanical Systems) technology, it enables precise environmental sensing to optimize indoor comfort and safety.

- __OLED 128 x 64 Display__
A compact and efficient display module that provides a clear interface for real-time data visualization, ensuring users can easily access air quality information.

- __Set of Various Screws & M3 Brass Inserts__
Essential hardware for securely assembling the device.

### Architecture
The architecture of PureSense is designed to provide seamless integration of hardware components, ensuring reliability and portability. At its core lies the FireBeetle ESP32-E IoT Microcontroller, which serves as the central processing unit, managing data collection, processing, and communication. Environmental data is continuously gathered by the BME680 Environmental Sensor, measuring temperature, humidity, air pressure, and VOC levels, alongside the MH-Z14A CO2 Sensor, which monitors carbon dioxide levels. This information is processed by the ESP32 and displayed in real-time on the OLED 128 x 64 Display, allowing users to instantly assess air quality.

Wireless connectivity is a key feature of the architecture, enabled by the ESP32's built-in Wi-Fi module. This allows the device to transmit data to external platforms for remote monitoring, creating opportunities for cloud-based analytics and broader integrations. The hardware assembly is compact and robust, constructed with a transparent 2mm acrylic casing that ensures both visibility and protection of the internal components. Secured with M3 brass inserts and screws, the design is both durable and easy to maintain, making PureSense ideal for portable use.

## Software
The software of PureSense is developed to maximize functionality while maintaining user-friendliness and efficiency. The ESP32 microcontroller is programmed using the Arduino IDE, which provides a flexible platform for integrating the various sensors and components. Custom code retrieves data from the BME680 and MH-Z14A CO2 sensors, processing it to display temperature, humidity, air pressure, VOC levels, and CO2 levels accurately.

Real-time data is dynamically presented on the OLED display, giving users immediate insights into the air quality of their environment. Additionally, the software is designed to support optional cloud integration, enabling remote data storage and monitoring for more comprehensive air quality management. Power efficiency is a critical feature of the system, with the ESP32 optimized for low-power operation to extend battery life and ensure sustained performance.

This combination of advanced hardware and thoughtfully developed software ensures that PureSense is not only effective in monitoring indoor air quality but also scalable and adaptable for a variety of applications.
