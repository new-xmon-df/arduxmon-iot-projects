# WEMOS D1 MINI **v4**
#### (older v1, v2, v3)

## Overview
The WEMOS D1 MINI boards are compact and powerful ESP8266-based microcontrollers. They offer Wi-Fi connectivity and a small form factor, making them ideal for IoT projects that require wireless communication.

[<img src="pictures/d1_mini_v4.0.0_1_16x16.png" width="300" alt="top view"/>](pictures/d1_mini_v4.0.0_1_16x16.png)
[<img src="pictures/d1_mini_v4.0.0_2_16x16.png" width="300" alt="bottom view"/>](pictures/d1_mini_v4.0.0_2_16x16.png)

## Features
- 11 digital IO, interrupt/pwm/I2C/one-wire supported(except D0)
- 1 analog input(3.2V max input)
- Type-C USB Port
- LOLIN I2C Port
- Compatible with MicroPython, Arduino, nodemcu

## Technical Specs
|                   |             |
|-------------------|-------------|
| Operating Voltage | 3.3V        |
| Digital I/O Pins  | 11          |
| Analog Input Pins | 1(3.2V Max) |
| Clock Speed       | 80/160MHz   |
| Flash             | 4M Bytes    |
| Size              | 34.2*25.6mm |
| Weight            | 3g          |

## Pinout
| Pin | Function                     | ESP-8266 Pin |
|-----|------------------------------|--------------|
| RST | Reset                        | RST          |
| A0  | Analog input, max 3.2V       | A0           |
| D0  | IO                           | GPIO16       |
| D5  | IO, SCK                      | GPIO14       |
| D6  | IO, MISO                     | GPIO12       |
| D7  | IO, MOSI                     | GPIO13       |
| D8  | IO, 10k Pull-down, SS        | GPIO15       |
| 3V3 | 3.3V                         | 3.3V         |
| TX  | TXD                          | TXD          |
| RX  | RXD                          | RXD          |
| D1  | IO, SCL                      | GPIO5        |
| D2  | IO, SDA                      | GPIO4        |
| D3  | IO, 10k Pull-up              | GPIO0        |
| D4  | IO, 10k Pull-up, BUILTIN_LED | GPIO2        |
| G   | Ground                       | GND          |
| 5V  | 5V                           | -            |

[<img src="wemos-d1-mini-pinout.png" width="1000" alt="PINOUT"/>](wemos-d1-mini-pinout.png)

## Using with ESPHome
The WEMOS D1 Mini V4 can be easily integrated with ESPHome for use in Home Assistant. Here are the basic steps to get started:

1. **Install ESPHome**: Follow the [installation guide](https://esphome.io/guides/installing_esphome.html) on the ESPHome website.
2. **Create a new configuration file**: Create a YAML file for your WEMOS D1 Mini V4. Here is an example configuration:

    ```yaml
    esphome:
      name: wemos_d1_mini_v4
      friendly_name: WEMOS D1 MINI V4
      comment: Template for this board
   
    esp8266:
      board: d1_mini

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
        name: "Wemos D1 Mini V4 Switch"
        pin: GPIO16
    ```

3. **Upload the configuration**: Use the ESPHome command line or the web interface to upload the configuration to your WEMOS D1 Mini V4.
4. **Integrate with Home Assistant**: Once the configuration is uploaded, the device will automatically appear in Home Assistant.

For detailed instructions and more configuration options, refer to the [ESPHome documentation](https://esphome.io/).

## DOWNLOAD FILES

Here I share the CAD program files.

- [**KICAD**](downloads/KICAD-WEMOS_D1_MINI.zip): Files for KiCad 6, includes symbol, footprint and 3D.
- [**KICAD template**](downloads/KICAD-PROJECT-TEMPLATE-ESP8266-WEMOS_D1_MINI.zip): Files for KiCad template.

## Documentation Links
- [Schematic v4](pdf/sch_d1_mini_v4.0.0.pdf)
- [Official WEMOS D1 MINI Documentation](https://www.wemos.cc/en/latest/d1/d1_mini.html)

## Versions
- **v4.0** (current)
- **v3.1**
- **v3.0**
- **v2.0**
- **v1.0**


[All boards comparative](../../Docs/comparative-boards.md)