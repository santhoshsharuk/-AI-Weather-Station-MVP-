# 🌦️ AI Weather Station MVP using Arduino

A minimal AI-enhanced weather station built with Arduino UNO that collects temperature, humidity, and atmospheric pressure data, and provides a basic weather forecast using rule-based logic.

## 🚀 Project Overview

This MVP (Minimum Viable Product) version of the weather station demonstrates how microcontrollers can gather environmental data and apply basic AI-like decision-making to produce simple weather predictions such as "Rain Possible" or "Clear Day".

## 📦 Components Used

| Component                | Description                                  |
|--------------------------|----------------------------------------------|
| Arduino UNO              | Main microcontroller                         |
| DHT11 Sensor             | Measures temperature and humidity            |
| BMP180 Sensor            | Measures atmospheric pressure                |
| Breadboard + Jumper Wires| For prototyping and connections              |
| USB Cable                | Power and programming interface              |

## 🔌 Circuit Connections

### DHT11 Sensor
- VCC → 5V  
- GND → GND  
- Data → Digital Pin 2  

### BMP180 Sensor
- VCC → 3.3V  
- GND → GND  
- SDA → A4  
- SCL → A5  

## 🧠 Features

- 📡 Live temperature, humidity, and pressure readings  
- 🧠 Basic AI (rule-based) forecast:
  - High humidity + low pressure → "Rain Possible"
  - Low humidity + high pressure → "Clear Day"
  - Otherwise → "Stable Weather"
- 🖥 Output displayed on the Arduino Serial Monitor

## 💻 Sample Output

```
Temp: 28.5 °C  
Humidity: 85.0 %  
Pressure: 998.4 hPa  
Forecast: Rain Possible  
--------------------
```

## 🧪 How to Use

1. Connect the sensors to Arduino as per the above circuit.
2. Upload the provided Arduino sketch.
3. Open the Serial Monitor (baud rate: 9600) to view live weather readings and forecast.
4. Observe weather trend prediction every 5 seconds.

## 🔮 Future Enhancements

- Add LCD or OLED display for local viewing
- Store historical data on SD card
- Train and deploy machine learning model for better prediction
- Add ESP8266 module for IoT dashboard access

## 📜 License

This project is open-source and free to use for learning and experimentation.
