# Smart Irrigation System

The **Smart Irrigation System** is an Arduino Uno-based project designed to maintain plant health by automatically monitoring soil humidity, atmospheric temperature, and water levels. The system dynamically controls water supply to ensure plants are hydrated, while also displaying real-time humidity and temperature data on a screen.

---

## Features
- **Automated Watering**: Uses a water level sensor to regulate the water supply based on soil moisture.
- **Real-Time Monitoring**: Displays soil humidity and atmospheric temperature on an LCD or OLED screen.
- **Environmentally Friendly**: Reduces water wastage by watering only when necessary.
- **User-Friendly**: Easy setup and monitoring through a digital display.

---

## Components Required
- **Arduino Uno**
- **Humidity and Temperature Sensor** (e.g., DHT11 or DHT22)
- **Water Level Sensor**
- **Relay Module** (for controlling the water pump)
- **Water Pump**
- **LCD or OLED Display**
- **Power Supply**
- **Connecting Wires and Breadboard**

---

## How It Works
1. **Data Collection**:  
   - The humidity and temperature sensor (DHT11/DHT22) measures atmospheric conditions.  
   - The water level sensor checks soil moisture levels.  

2. **Processing**:  
   - The Arduino Uno processes the sensor data and determines if the soil requires watering.  

3. **Watering Automation**:  
   - If the soil moisture falls below a certain threshold, the relay activates the water pump to hydrate the plants.  

4. **Display Updates**:  
   - The LCD or OLED screen shows real-time humidity and temperature readings for easy monitoring.

---

## Getting Started

### Hardware Setup
1. Connect the **DHT11/DHT22 sensor** to the Arduino Uno.  
   - Pin 1 → VCC  
   - Pin 2 → Digital Pin (e.g., D2)  
   - Pin 4 → GND  

2. Connect the **Water Level Sensor** to the Arduino Uno.  
   - VCC → Arduino 5V  
   - GND → Arduino GND  
   - Signal → Analog Pin (e.g., A0)  

3. Connect the **Relay Module** to control the water pump.  
   - VCC → Arduino 5V  
   - GND → Arduino GND  
   - Signal → Digital Pin (e.g., D3)  

4. Connect the **LCD/OLED Display** to the Arduino Uno.  
   - Follow the connection diagram based on your display type.  

5. Wire the water pump to the relay module.

---

### Software Setup
1. Install the required libraries in Arduino IDE:  
   - **DHT Sensor Library**: [Download Here](https://github.com/adafruit/DHT-sensor-library)  
   - **LiquidCrystal_I2C Library**: [Download Here](https://github.com/fdebrabander/Arduino-LiquidCrystal-I2C-library) (if using an I2C LCD)  

2. Open the Arduino IDE and load the program for the Smart Irrigation System.  

3. Adjust the soil moisture threshold and temperature settings in the code as needed.  

4. Upload the program to the Arduino Uno.  

---

## Demonstration Video
Watch the Smart Irrigation System in action:

[![Smart Irrigation System Demo](path-to-thumbnail-image.jpg)](path-to-video.mp4)  
*Click the image to play the video.*

---

## Applications
- Home Gardens
- Greenhouses
- Agricultural Fields
- Indoor Plants

---

## Benefits
- **Efficient Water Management**: Avoids overwatering and conserves water.  
- **Plant Growth Optimization**: Maintains the ideal environmental conditions for plants.  
- **Convenience**: Reduces manual effort and ensures consistent plant care.  

---

## Future Enhancements
- **IoT Integration**: Add Wi-Fi or Bluetooth modules for remote monitoring and control.  
- **Weather Forecasting**: Include weather data to optimize watering schedules.  
- **Solar Power**: Make the system energy-independent with solar panels.
