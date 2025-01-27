# WEMOS D1 MINI ESP32 V2.0

## Description
The WEMOS D1 Mini ESP32 Development Board is the successor of the D1 Mini with the ESP8266. Its pins are compatible with all modules designed for the D1 Mini ESP8266 and incorporate all the additional improvements of the powerful ESP32.

The ESP32 integrates Wi-Fi and Bluetooth BLE, making it ideal for developing IoT products. Wi-Fi allows for medium-range communication and connection to a LAN network and, through a router, to the Internet. Bluetooth enables direct connection to another device such as a cellphone.

The ESP32 chip's standby current is less than 5 µA, making it suitable for portable electronic applications with batteries.

At the core of this module is the ESP32-D0WDQ6 chip. The integrated chip is designed to be scalable and adaptable, featuring two CPU cores that can be controlled individually and a clock frequency adjustable from 80 MHz to 240 MHz. It also features an Xtensa® LX6 dual-core processor.

The D1 Mini ESP32 is equipped with a CP2104 USB-to-Serial converter, which provides virtual COM port functionality, simplifying serial communication setup with computers. 

The board includes pre-installed firmware for interpreted language support and allows programming with Arduino IDE or ESP-IDF. It supports breadboard mounting and is compatible with shields specifically designed for the D1 Mini ESP32.

## Features
| Feature                                        | Description                                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Robust design                                  | ESP32 is capable of reliable operation in industrial environments, with an operating temperature range from -40°C to +125°C.                                            |
| Ultra-low power consumption                    | Designed for mobile devices, wearable electronics, and IoT applications, ESP32 achieves ultra-low power consumption with a combination of various proprietary software. |
| High level of integration                      | ESP32 is highly integrated with built-in antenna switches, RF balun, power amplifiers, low-noise amplifiers, filters, and power management modules.                     |
| Wi-Fi and Bluetooth BLE connectivity           | Integrates Wi-Fi and Bluetooth BLE, allowing for a wide range of IoT applications and direct connections to other devices.                                              |
| Compatible with Arduino IDE                    | Can be programmed using the Arduino IDE, providing access to a wide range of resources and libraries available in the Arduino ecosystem.                                |
| Wide range of GPIOs, UART, SPI, I2C interfaces | Offers multiple GPIOs, UART, SPI, and I2C interfaces for connecting various sensors and peripherals.                                                                    |
| Capacitive touch sensors                       | Features capacitive touch sensors on 10 GPIOs, enabling the creation of touch-sensitive interfaces.                                                                     |
| SD card interface                              | Includes an interface for SD cards, allowing for additional storage options.                                                                                            |
| Integrated TCP/IP protocol stack               | Comes with an integrated TCP/IP protocol stack, simplifying network communication.                                                                                      |
| FCC/CE/IC/TELEC/KCC/SRRC/NCC certified         | Certified for compliance with FCC/CE/IC/TELEC/KCC/SRRC/NCC regulations.                                                                                                 |
| Wide range of network protocols supported      | Supports IPv4, IPv6, SSL, TCP, UDP, HTTP, FTP, MQTT, and other network protocols.                                                                                       |
| Audio support for CVSD and SBC formats         | Provides support for CVSD and SBC audio formats.                                                                                                                        |
| Hall effect sensor                             | Includes a built-in Hall effect sensor to detect changes in magnetic fields.                                                                                            |
| Internal temperature sensor                    | Features an internal temperature sensor for detecting relative changes in temperature, suitable for calibration purposes.                                               |

## Technical Specifications
| Specification                | Details                               |
|------------------------------|---------------------------------------|
| Operating Voltage            | 5V DC (4.5~6V)                        |
| Operating Current            | ~80mA (source >500mA)                 |
| Logic Level (Inputs/Outputs) | 3.3V                                  |
| SoC                          | ESP32 (ESP32-D0WDQ6)                  |
| CPU                          | Dual-core Xtensa® LX6 (32-bit)        |
| Clock Frequency              | 80MHz to 240MHz                       |
| SRAM                         | 520KB                                 |
| External Flash Memory        | 4MB                                   |
| Digital GPIO Pins            | 34 (including all peripherals)        |
| GPIO Max Output Current      | 40mA per pin                          |
| UART                         | 2                                     |
| SPI                          | 3                                     |
| I2C                          | 2                                     |
| I2S                          | Yes                                   |
| CAN                          | Yes                                   |
| Capacitive Touch Sensors     | 10                                    |
| ADC                          | 18 channels (12-bit resolution)       |
| DAC                          | 2 channels (8-bit resolution)         |
| RTC GPIO Support             | Yes (usable in deep sleep mode)       |
| Wi-Fi Protocol               | 802.11 b/g/n (802.11n up to 150 Mbps) |
| Bluetooth Protocols          | V4.2 BLE and Classic                  |
| Antenna Type                 | PCB                                   |
| Dimensions                   | 39x28x6 mm                            |

## Pinout
| Pin Number | Function              | ADC       | SPI       | DAC   | TOUCH | UART/I2C/PWM |
|------------|-----------------------|-----------|-----------|-------|-------|--------------|
| EN         | Enable                | -         | -         | -     | -     | -            |
| GPIO0      | Digital I/O           | ADC2_CH1  | -         | -     | T1    | **✓**        |
| GPIO2      | Digital I/O           | ADC2_CH2  | -         | -     | T2    | **✓**        |
| GPIO4      | Digital I/O           | ADC2_CH0  | -         | -     | T0    | **✓**        |
| GPIO12     | Digital I/O           | ADC2_CH5  | HSPI_CLK  | -     | T5    | **✓**        |
| GPIO13     | Digital I/O           | ADC2_CH4  | HSPI_MISO | -     | T4    | **✓**        |
| GPIO14     | Digital I/O           | ADC2_CH6  | HSPI_MOSI | -     | T6    | **✓**        |
| GPIO15     | Digital I/O           | ADC2_CH3  | HSPI_CS0  | -     | T3    | **✓**        |
| GPIO16     | Digital I/O           | ADC2_CH7  | -         | -     | -     | **✓**        |
| GPIO17     | Digital I/O           | ADC2_CH8  | -         | DAC_1 | -     | **✓**        |
| GPIO18     | Digital I/O           | ADC2_CH9  | VSPI_CLK  | DAC_2 | -     | **✓**        |
| GPIO19     | Digital I/O           | ADC2_CH10 | VSPI_MISO | -     | -     | **✓**        |
| GPIO21     | Digital I/O (I2C SDA) | -         | -         | -     | -     | **✓**        |
| GPIO22     | Digital I/O (I2C SCL) | -         | -         | -     | -     | **✓**        |
| GPIO23     | Digital I/O           | ADC2_CH11 | VSPI_MOSI | -     | -     | **✓**        |
| GPIO25     | Digital I/O           | ADC2_CH12 | -         | DAC_1 | -     | **✓**        |
| GPIO26     | Digital I/O           | ADC2_CH13 | -         | DAC_2 | -     | **✓**        |
| GPIO27     | Digital I/O           | ADC2_CH14 | -         | -     | T7    | **✓**        |
| GPIO32     | Digital I/O           | ADC1_CH4  | -         | -     | T9    | **✓**        |
| GPIO33     | Digital I/O           | ADC1_CH5  | -         | -     | T8    | **✓**        |
| GPIO34     | Digital Input (ADC)   | ADC1_CH6  | -         | -     | -     | -            |
| GPIO35     | Digital Input (ADC)   | ADC1_CH7  | -         | -     | -     | -            |
| GPIO36     | Digital Input (ADC)   | ADC1_CH0  | -         | -     | -     | -            |
| GPIO39     | Digital Input (ADC)   | ADC1_CH3  | -         | -     | -     | -            |
| 3.3V       | Power                 | -         | -         | -     | -     | -            |
| GND        | Ground                | -         | -         | -     | -     | -            |

[<img src="wemos-d1-mini-esp32-pinout.png" width="1000" alt="PINOUT"/>](wemos-d1-mini-esp32-pinout.png)

## Using with ESPHome
The WEMOS D1 Mini ESP32 can be easily integrated with ESPHome for use in Home Assistant. Here are the basic steps to get started:

1. **Install ESPHome**: Follow the [installation guide](https://esphome.io/guides/installing_esphome.html) on the ESPHome website.
2. **Create a new configuration file**: Create a YAML file for your WEMOS D1 Mini ESP32. Here is an example configuration:

    ```yaml
    esphome:
      name: wemos_d1_mini_esp32
      friendly_name: WEMOS D1 MINI ESP32
      comment: Template for this board
   
    esp32:
      board: wemos_d1_mini32 # https://docs.platformio.org/en/latest/boards/espressif32/wemos_d1_mini32.html
      framework:
        type: arduino

    wifi:
      ssid: "your_SSID"
      password: "your_PASSWORD"

    # Enable logging
    logger:

    # Enable Home Assistant API
    api:
      password: "your_API_password"

    ota:
      password: "your_OTA_password"

    # Example configuration entry for a GPIO switch
    switch:
      - platform: gpio
        name: "Wemos D1 Mini ESP32 Switch"
        pin: GPIO16
    ```

3. **Upload the configuration**: Use the ESPHome command line or the web interface to upload the configuration to your WEMOS D1 Mini ESP32.
4. **Integrate with Home Assistant**: Once the configuration is uploaded, the device will automatically appear in Home Assistant.

For detailed instructions and more configuration options, refer to the [ESPHome documentation](https://esphome.io/).

## DOWNLOAD FILES

Here I share the CAD program files.

- [**KICAD**](downloads/KICAD-WEMOS_D1_MINI_ESP32.zip): Files for KiCad 6, includes symbol, footprint and 3D.
- [**KICAD template**](downloads/KICAD-PROJECT-TEMPLATE-ESP32-WEMOS_D1_MINI_ESP32.zip): Files for KiCad template.

## Documentation Links
- ![Pending Doc](https://img.shields.io/badge/Schematic-Pending_Doc-blue)
- ![Official WEMOS D1 MINI ESP32 Documentation](https://www.wemos.cc/en/latest/d1/d1_mini32.html)

[All boards comparative](../../Docs/comparative-boards.md)
