# Flood Detection System

Smart water level monitoring system using ESP32 with multiple warning alerts.

## Features
- Real-time water level monitoring with HC-SR04 sensor
- OLED display for status and readings
- Buzzer + LED warnings when threshold exceeded
- Blynk app remote monitoring
- Web interface for configuration
- Physical button controls

## Hardware
- ESP32 board
- HC-SR04 ultrasonic sensor
- 1.3" OLED display (SH1106)
- Buzzer, LED, Relay
- 3 push buttons

## Pin Connections
| Component | Pin |
|-----------|-----|
| HC-SR04 Trig/Echo | 19/18 |
| OLED SDA/SCL | 21/22 |
| LED | 33 |
| Buzzer | 2 |
| Buttons | 32,35,34 |

## Setup
1. Install Arduino IDE + ESP32 support
2. Install libraries: `BlynkSimpleEsp32`, `Adafruit_SH110X`, `HCSR04`, `ESPAsyncWebServer`
3. Configure Blynk credentials in code
4. Upload code to ESP32
5. Connect hardware and power on

## Usage
- **SET button**: Enter configuration mode
- **UP/DOWN buttons**: Adjust values
- Configure sensor height and warning threshold
- System automatically monitors and alerts when water level exceeds threshold
