# ESP32 Marauder for ILI9341 Display

This repository contains a version of the ESP32 Marauder, customized to work with ILI9341 displays. The project provides an interface and various tools for network analysis and testing directly on the ESP32 platform.

## Features
- Network analysis and scanning functionalities.
- UI compatible with ILI9341 displays.
- Support for peripherals including SD Card, GPS modules, and LEDs.
- Interactive menu system for easy navigation.

## Setup
1. Open the project folder in the Arduino IDE or PlatformIO.
2. Select your specific ESP32 board in the settings.
3. Ensure all the required libraries (like those for the ILI9341 display, SD card, etc.) are installed.
4. Compile and upload the main sketch (`esp32_marauder_for_ILI9341_Display.ino`) to your ESP32 device.

## File Structure
- `esp32_marauder_for_ILI9341_Display.ino`: Main application entry point.
- `Display.cpp` / `Display.h`: Display driver and rendering logic.
- `MenuFunctions.cpp` / `MenuFunctions.h`: Interactive UI and menu handling.
- `WiFiScan.cpp` / `WiFiScan.h`: Wireless scanning and analysis logic.
- `SDInterface.cpp` / `SDInterface.h`: SD card interaction and logging.
- `GpsInterface.cpp` / `GpsInterface.h`: GPS data handling.

## Disclaimer
This tool is intended for educational purposes, authorized auditing, and testing only. Users are responsible for complying with all applicable local, state, and federal laws. Never use these tools on networks for which you do not have explicit permission.
