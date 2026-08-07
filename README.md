# 🦅 ESP32 Marauder for ILI9341 Display

![Educational Purpose Only](https://img.shields.io/badge/Purpose-Educational%20Only-red.svg)
![Platform](https://img.shields.io/badge/Platform-ESP32-blue.svg)
![Display](https://img.shields.io/badge/Display-ILI9341-green.svg)

> **⚠️ Disclaimer:** This project is for **educational purposes only**. The user is solely responsible for compliance with all local, state, and federal laws. Never use these tools on networks for which you do not have explicit permission.

Welcome to the **ESP32 Marauder** tailored specifically for **ILI9341 Displays**. This project provides a powerful interface and an array of tools for network analysis, auditing, and testing directly on the ESP32 platform.

---

## 🌟 Key Features

- **Advanced Network Analysis**: Robust Wi-Fi and Bluetooth scanning and auditing capabilities.
- **ILI9341 UI Compatibility**: A responsive, touch-friendly interactive menu system optimized for ILI9341 displays.
- **Hardware Integrations**: Full support for SD Card logging, GPS modules, and WS2812 LEDs.
- **Portable & Compact**: Run complex network testing operations from a small, self-contained microcontroller.

---

## 🔌 Hardware Wiring & Pinout Guide

To ensure proper functionality, connect your hardware components to the ESP32 according to the tables below.

### 📺 Display & Touch (ILI9341)
| ILI9341 Pin | Label | ESP32 Pin |
|:---:|:---|:---|
| 1 | **VCC** | 3.3V |
| 2 | **GND** | GND |
| 3 | **CS** | D17 (TXD 2) |
| 4 | **RESET** | D5 |
| 5 | **DC** | D16 (RXD 2) |
| 6 | **SDI (MOSI)** | D23 |
| 7 | **SCK** | D18 |
| 8 | **LED** | D32 |
| 9 | **SDO (MISO)** | D19 |
| 10 | **T_CLK** | D18 |
| 11 | **T_CS** | D21 |
| 12 | **T_DIN** | D23 |
| 13 | **T_DO** | D19 |
| 14 | **T_IRQ** | *Not Connected* |

### 💾 SD Card Module
| SD Card Pin | Label | ESP32 Pin |
|:---:|:---|:---|
| 1 | **CS** | D12 |
| 2 | **MOSI** | D23 |
| 3 | **MISO** | D19 |
| 4 | **SCK** | D18 |
*(Note: VCC and GND should be connected to 3.3V and GND respectively)*

### 🌍 GPS Module
| GPS Pin | Label | ESP32 Pin |
|:---:|:---|:---|
| 1 | **VIN** | 3.3V |
| 2 | **GND** | GND |
| 3 | **TX** | D4 |
| 4 | **RX** | D13 |

### 💡 LED WS2812
| LED Pin | Label | ESP32 Pin |
|:---:|:---|:---|
| 1 | **DIN** | D25 |
| 2 | **VCC** | 3.3V |
| 3 | **GND** | GND |
| 4 | **DOUT** | *Not Connected* |

---

## 🚀 Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/VenomDevX/ESP32-Marauder.git
   ```
2. **Open the Project**:
   Open the folder in the **Arduino IDE** or **PlatformIO**.
3. **Select Board**:
   Choose your specific ESP32 board in the IDE settings.
4. **Install Dependencies**:
   Ensure all required libraries for the ILI9341 display, SD card, GPS, etc., are installed via the Library Manager.
5. **Compile & Upload**:
   Compile the main sketch (`esp32_marauder_for_ILI9341_Display.ino`) and upload it to your ESP32 device.

---

## 📂 File Structure Overview

- `esp32_marauder_for_ILI9341_Display.ino`: Core application entry point.
- `Display.cpp` / `.h`: Display driver and UI rendering logic.
- `MenuFunctions.cpp` / `.h`: Interactive UI and menu state management.
- `WiFiScan.cpp` / `.h`: Wireless scanning, analysis, and network interactions.
- `SDInterface.cpp` / `.h`: SD card initialization and data logging.
- `GpsInterface.cpp` / `.h`: NMEA parsing and GPS data handling.

---

*For educational and authorized auditing purposes only. Stay safe, and test responsibly!*
