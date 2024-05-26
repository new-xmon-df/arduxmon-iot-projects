# NODEMCU32 ESP-WROOM-32

## Overview

The NODEMCU32 ESP-WROOM-32 is an open-source firmware development module based on the ESP32 chip. It integrates a dual-core 32-bit Tensilica Xtensa processor running at up to 240MHz, Wi-Fi, and Bluetooth connectivity. It provides extensive features and compatibility with various development environments, making it an ideal choice for Internet of Things (IoT) projects.

[ESP32 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/hw-reference/index.html).

[<img src="pictures/ESP32-DEVKIT-38PINS-front.jpg" width="300" alt="top view"/>](pictures/ESP32-DEVKIT-38PINS-front.jpg)
[<img src="pictures/ESP32-DEVKIT-38PINS-back.jpg" width="300" alt="bottom view"/>](pictures/ESP32-DEVKIT-38PINS-back.jpg)

## Features

- **SoC:** ESP32-WROOM-32
- **CPU:** Xtensa® single/dual-core 32-bit LX6
- **Clock Frequency:** 80MHz / 240MHz
- **RAM:** 520kB
- **External Flash Memory:** 4MB
- **I/O Pins:** 34
- **ADC Channels:** 18
- **ADC Resolution:** 12-bit
- **DAC Channels:** 2
- **DAC Resolution:** 8-bit
- **Communication Interfaces:** SPI, I2C, I2S, CAN, UART
- **Wi-Fi Protocols:** 802.11 b/g/n (up to 150 Mbps)
- **Wi-Fi Frequency:** 2.4 GHz - 2.5 GHz
- **Bluetooth:** V4.2 - BLE and Classic Bluetooth
- **Wireless Antenna:** PCB
- **Dimensions:** 56x28x13mm (2.2x1.1x0.5in)

## Usage

The module can be powered through the micro USB port with 5V or through the 3.3V pin with caution. Using 5V on the 3.3V pin may damage the module. It features the CP2102 USB to UART controller for USB-Serial communication.

It can be programmed using various software, programming languages, frameworks, libraries, and examples, including Espressif IoT Development Framework (ESP-IDF), Arduino IDE (C++), MicroPython, Lua, and more.

The NODEMCU32 ESP-WROOM-32 is designed for prototyping IoT projects, featuring easy connectivity with sensors and actuators via Wi-Fi and Bluetooth.

## Technical Specs

|                            |                                  |
|----------------------------|----------------------------------|
| Power Supply Voltage (USB) | 5V DC                            |
| Input/Output Voltage       | 3.3V DC                          |
| Operating Current (min.)   | 500mA                            |
| Clock Frequency Range      | 80MHz / 240MHz                   |
| RAM                        | 520kB                            |
| External Flash Memory      | 4MB                              |
| I/O Pins                   | 34                               |
| ADC Channels               | 18                               |
| ADC Resolution             | 12-bit                           |
| DAC Channels               | 2                                |
| DAC Resolution             | 8-bit                            |
| Communication Interfaces   | SPI, I2C, I2S, CAN, UART         |
| Wi-Fi Protocols            | 802.11 b/g/n (up to 150 Mbps)    |
| Wi-Fi Frequency            | 2.4 GHz - 2.5 GHz                |
| Bluetooth                  | V4.2 - BLE and Classic Bluetooth |
| Wireless Antenna           | PCB                              |
| Dimensions                 | 56x28x13mm (2.2x1.1x0.5in)       |

## Pins Description

Just like a normal Arduino board, the ESP32 Dev Kit C V2 has digital input/output pins (GPIO pins - General Purpose Input/Output pins). These digital input/outputs operate at 3.3V.

<span style="color:#ff0000">**5V voltage must not be connected to any ESP32 chip pins!**</span>

The pins are not 5V tolerant, applying more than 3.3V on any pin will destroy the chip.

The GPIO pins 34 to 39 are GPIs – input only pins. These pins do not have internal pull-ups or pull-down resistors. They cannot be used as outputs, so use these pins only as inputs: GPIO 34, GPIO 35, GPIO 36, GPIO 39

There is an integrated SPI flash on the ESP-WROOM-32 chip. The pins GPIO6 to GPIO 11 are exposed in certain ESP32 development boards. These pins are connected to the integrated SPI flash on the chip and are not recommended for other uses.

GPIO 6 (SCK/CLK), GPIO 7 (SDO/SD0), GPIO 8 (SDI/SD1), GPIO 9 (SHD/SD2), GPIO 10 (SWP/SD3), GPIO 11 (CSC/CMD).

## Capacitive Touch Sensor Pins

The ESP32 has 10 internal capacitive touch sensors. The capacitive touch pins can also be used to wake up the ESP32 from deep sleep. These internal touch sensors are connected to these GPIOs: T0 (GPIO 4), T1 (GPIO 0), T2 (GPIO 2), T3 (GPIO 15), T4 (GPIO 13), T5 (GPIO 12), T6 (GPIO 14), T7 (GPIO 27), T8 (GPIO 33), T9 (GPIO 32).

## Analog to Digital Converter Pins

The ESP32 has 18x12 bits ADC (Analog to Digital converter) input channels (while the ESP8266 only has 1x 10 bits ADC). These are the GPIOs that can be used as ADC and respective channels:

ADC1_CH0 (GPIO 36), ADC1_CH1 (GPIO 37), ADC1_CH2 (GPIO 38), ADC1_CH3 (GPIO 39), ADC1_CH4 (GPIO 32), ADC1_CH5 (GPIO 33), ADC1_CH6 (GPIO 34), ADC1_CH7 (GPIO 35), ADC2_CH0 (GPIO 4), ADC2_CH1 (GPIO 0), ADC2_CH2 (GPIO 2), ADC2_CH3 (GPIO 15), ADC2_CH4 (GPIO 13), ADC2_CH5 (GPIO 12), ADC2_CH6 (GPIO 14), ADC2_CH7 (GPIO 27), ADC2_CH8 (GPIO 25), ADC2_CH9 (GPIO 26).

## Digital to Analog Converter Pins

There are 2x8 bits DAC (Digital to Analog converter) channels on the ESP32 to convert digital signals into analog voltage signal outputs. These are the DAC channels:

DAC1 (GPIO 25), DAC2 (GPIO 26).

## Real Time Clock GPIO Pins

There is RTC (Real time clock) GPIO support on the ESP32. The GPIOs routed to the RTC low-power subsystem can be used when the ESP32 is in deep sleep. These RTC GPIOs can be used to wake up the ESP32 from deep sleep when the Ultra Low Power (ULP) coprocessor is running. The following GPIOs can be used as an external wake-up source:

RTC_GPIO0 (GPIO 36), RTC_GPIO3 (GPIO 39), RTC_GPIO4 (GPIO 34), RTC_GPIO5 (GPIO 35), RTC_GPIO6 (GPIO 25), RTC_GPIO7 (GPIO 26), RTC_GPIO8 (GPIO 33), RTC_GPIO9 (GPIO 32), RTC_GPIO10 (GPIO 4), RTC_GPIO11 (GPIO 0), RTC_GPIO12 (GPIO 2), RTC_GPIO13 (GPIO 15), RTC_GPIO14 (GPIO 13), RTC_GPIO15 (GPIO 12), RTC_GPIO16 (GPIO 14), RTC_GPIO17 (GPIO 27).

## PWM (Pulse Width Modulation) Pins

The ESP32 LED PWM (Pulse width modulation) controller has 16 independent channels that can be configured to generate PWM signals with different properties. All pins that can act as outputs can be used as PWM pins (GPIOs 34 to 39 cannot generate PWM). To set a PWM signal, you need to define these parameters in the code: Signal’s frequency, Duty cycle, PWM channel, GPIO where you want to output the signal.

## The I2C Interface Pins

The ESP32 has two I2C channels and any pin can be set as SDA or SCL. When using the ESP32 with the Arduino IDE, the default I2C pins are:

GPIO 21 (SDA), GPIO 22 (SCL).

## SPI Interface Pins

By default, the pin mapping for SPI pins is:

| SPI  | MOSI    | MISO    | CLK     | CS      |
|------|---------|---------|---------|---------|
| VSPI | GPIO 23 | GPIO 19 | GPIO 18 | GPIO 5  |
| HSPI | GPIO 13 | GPIO 12 | GPIO 14 | GPIO 15 |

## Strapping Pins

The following pins are used to put the ESP32 into bootloader or flashing mode: GPIO 0, GPIO 2, GPIO 4, GPIO 5 (must be HIGH during boot), GPIO 12 (must be LOW during boot), GPIO 15 (must be HIGH during boot).

Most development boards put the pins in the right state for flashing or boot mode. If some peripherals are connected to the strapping pins and the IDE is unable to upload the code or flash the ESP32, it may be because those peripherals are preventing the ESP32 from entering the right mode. After resetting, flashing, or booting, those pins work as expected.

## Pins HIGH at Boot

Some GPIOs change their state to HIGH or output PWM signals at boot or reset. This means that if outputs are connected to these GPIOs, this may get unexpected results when the ESP32 resets or boots. GPIO 1, GPIO 3, GPIO 5, GPIO 6 to GPIO 11 (connected to the ESP32 integrated SPI flash memory - not recommended for use), GPIO 14, GPIO 15.

## Enable (EN)

Enable (EN) is the 3.3V regulator’s enable pin. It has a pulled up state, and it needs to be connected to ground to disable the 3.3V regulator. This means that this pin can be connected to a push button to restart your ESP32, for example.

## USB to Serial Communication

The ESP32 Dev Kit C V2 has a microUSB connection port. It is made around the CP2102 chip made by Silicon Laboratories which allows USB to UART serial communication. The chip has the virtual COM port (VCP) feature that appears as a COM port in PC applications. The CP2102 UART interface implements all RS-232 signals, including control and handshaking signals, so existing system firmware does not need to be modified. To be able to use the ESP32, the driver has to be installed.

## Wi-Fi Communication

ESP32 Dev Kit C V2 has an integrated Wi-Fi communication interface and can operate in three different modes: Wi-Fi station, Wi-Fi access point, and both at the same time. It supports the following features:

* 802.11b and 802.11g data-rates
* 802.11n MCS0-7 in both 20MHz and 40MHz bandwidth
* 802.11n MCS32
* 802.11n 0.4µS guard-interval
* Data-rate up to 150 Mbps
* Receiving STBC 2x1
* Up to 21 dBm transmitting power
* Adjustable transmitting power
* Antenna diversity and selection (software-managed hardware)

## Bluetooth Communication

The ESP32 Dev Kit C V2 has an integrated Bluetooth Radio and supports the following features:

* Class-1, class-2 and class-3 transmit output powers and over 30 dB dynamic control range
* π/4 DQPSK and 8 DPSK modulation
* High performance in NZIF receiver sensitivity with over 98 dB dynamic range
* Class-1 operation without external PA
* Internal SRAM allows full speed data transfer, mixed voice and data, and full piconet operation
* Logic for forward error correction, header error control, access code correlation, CRC, demodulation, encryption bit stream generation, whitening and transmit pulse shaping
* ACL, SCO, eSCO and AFH
* A-law, µ-law and CVSD digital audio CODEC in PCM interface
* SBC audio CODEC
* Power management for low power applications
* SMP with 128-bit AES

Also, the Bluetooth Radio has support for the following communication interface protocols:

* UART HCI interface, up to 4 Mbps
* SDIO / SPI HCI interface
* I2C interface
* PCM / I2S audio interface

## Other Features

The ESP32-WROOM-32 chip has an integrated Hall Effect Sensor that detects changes in the magnetic field in its surroundings.

The Hall sensor is based on an N-carrier resistor. When the chip is in the magnetic field, the Hall sensor develops a small voltage on the resistor, which can be directly measured by the analog-digital converter (ADC), or amplified by the ultra-low noise analog pre-amplifier and then measured by the ADC.

The temperature sensor generates a voltage that varies with temperature. The voltage is internally converted via an analog-to-digital converter into a digital code. The temperature sensor has a range of -40°C to 125°C. As the offset of the temperature sensor varies from chip to chip due to process variation, together with the heat generated by the Wi-Fi circuitry itself (which affects measurements), the internal temperature sensor is only suitable for applications that detect temperature changes instead of absolute temperatures and for calibration purposes as well. However, if the user calibrates the temperature sensor and uses the device in a minimally powered-on application, the results could be accurate enough.

## Pinout
| Board pin name | Pin number | ADC    | Capacitive Touch | SPI     | UART  | I2C     | DAC   | RTC    | Strapping Pin      | PWM   | Notes                                                                                             |
|----------------|------------|--------|------------------|---------|-------|---------|-------|--------|--------------------|-------|---------------------------------------------------------------------------------------------------|
| 3V3            | -          | -      | -                | -       | -     | -       | -     | -      | -                  | -     | Power Supply: 3.3V                                                                                |
| EN             | -          | -      | -                | -       | -     | -       | -     | -      | Enable (EN), RESET | -     | Pulled up state, reset pin                                                                        |
| SP             | GPIO36     | ADC1_0 | -                | -       | -     | -       | -     | RTC_0  | -                  | -     | Analog to Digital Converter channel, External wake-up source                                      |
| SN             | GPIO39     | ADC1_3 | -                | -       | -     | -       | -     | RTC_3  | -                  | -     | Analog to Digital Converter channel, External wake-up source                                      |
| S34            | GPIO34     | ADC1_6 | -                | -       | -     | -       | -     | RTC_4  | -                  | -     | Analog to Digital Converter channel, External wake-up source                                      |
| S35            | GPIO35     | ADC1_7 | -                | -       | -     | -       | -     | RTC_5  | -                  | -     | Analog to Digital Converter channel, External wake-up source                                      |
| S32            | GPIO32     | ADC1_4 | TOUCH 9          | -       | -     | -       | -     | RTC_9  | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source                    |
| S33            | GPIO33     | ADC1_5 | TOUCH 8          | -       | -     | -       | -     | RTC_8  | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source                    |
| S25            | GPIO25     | ADC2_8 | -                | -       | -     | -       | DAC 1 | RTC_6  | -                  | **✓** | Analog to Digital Converter channel, Digital to Analog Converter channel, External wake-up source |
| S26            | GPIO26     | ADC2_9 | -                | -       | -     | -       | DAC 2 | RTC_7  | -                  | **✓** | Analog to Digital Converter channel, Digital to Analog Converter channel, External wake-up source |
| S27            | GPIO27     | ADC2_7 | TOUCH 7          | -       | -     | -       | -     | RTC_17 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source                    |
| S14            | GPIO14     | ADC2_6 | TOUCH 6          | SD CLK  | -     | -       | -     | RTC_16 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source, SPI CLK           |
| S12            | GPIO12     | ADC2_5 | TOUCH 5          | -       | -     | -       | -     | RTC_15 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source, SPI MOSI          |
| GND            | -          | -      | -                | -       | -     | -       | -     | -      | -                  | -     | Ground                                                                                            |
| S13            | GPIO13     | ADC2_4 | -                | -       | -     | -       | -     | RTC_14 | -                  | **✓** | Analog to Digital Converter channel, External wake-up source, SPI MISO                            |
| SD2            | GPIO9      | -      | -                | SPI D2  | -     | -       | -     | -      | -                  | **✓** | SPI Data line 2                                                                                   |
| SD3            | GPIO10     | -      | -                | SPI D3  | -     | -       | -     | -      | -                  | **✓** | SPI Data line 3                                                                                   |
| GND            | GPIO11     | -      | -                | SPI CMD | -     | -       | -     | -      | -                  | **✓** | SPI CMD                                                                                           |
| 5V             | -          | -      | -                | -       | -     | -       | -     | -      | -                  | -     | Power Supply: 5V                                                                                  |
| GND            | -          | -      | -                | -       | -     | -       | -     | -      | -                  | -     | Ground                                                                                            |
| G23            | GPIO23     | -      | -                | MOSI    | -     | -       | -     | -      | -                  | **✓** | SPI MOSI                                                                                          |
| G22            | GPIO22     | -      | -                | -       | -     | I2C1 CL | -     | -      | -                  | **✓** | I2C Clock                                                                                         |
| TXD            | GPIO1      | -      | -                | -       | U0 TX | -       | -     | -      | -                  | **✓** | UART Transmit                                                                                     |
| RXD            | GPIO3      | -      | -                | -       | U0 RX | -       | -     | -      | -                  | **✓** | UART Receive                                                                                      |
| G21            | GPIO21     | -      | -                | -       | -     | I2C1 DA | -     | -      | -                  | **✓** | I2C Data                                                                                          |
| GND            | -          | -      | -                | -       | -     | -       | -     | -      | -                  | -     | Ground                                                                                            |
| G19            | GPIO19     | -      | -                | MISO    | -     | -       | -     | -      | -                  | **✓** | SPI MISO                                                                                          |
| G18            | GPIO18     | -      | -                | CLK     | -     | -       | -     | -      | -                  | **✓** | Clock signal                                                                                      |
| G5             | GPIO5      | -      | -                | SS      | -     | -       | -     | -      | -                  | **✓** | SPI Slave Select                                                                                  |
| G17            | GPIO17     | -      | -                | -       | U2 TX | -       | -     | -      | -                  | **✓** | UART2 Transmit                                                                                    |
| G16            | GPIO16     | -      | -                | -       | U2 RX | -       | -     | -      | -                  | **✓** | UART2 Receive                                                                                     |
| G4             | GPIO4      | ADC2_0 | TOUCH 0          | SD D1   | -     | -       | -     | RTC_10 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source, SPI Data line 1   |
| G0             | GPIO0      | ADC2_1 | TOUCH 1          | -       | -     | -       | -     | RTC_11 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source                    |
| G2             | GPIO2      | ADC2_2 | TOUCH 2          | SD D0   | -     | -       | -     | RTC_12 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source, SPI MOSI          |
| G15            | GPIO15     | ADC2_3 | TOUCH 3          | SD CMD  | -     | -       | -     | RTC_13 | -                  | **✓** | Analog to Digital Converter channel, Capacitive Touch, External wake-up source, SPI Command       |
| SD1            | GPIO8      | -      | -                | SPI D1  | -     | -       | -     | -      | -                  | **✓** | SPI Data line 1                                                                                   |
| SD0            | GPIO7      | -      | -                | SPI D0  | -     | -       | -     | -      | -                  | **✓** | SPI Data line 0                                                                                   |
| CLK            | GPIO6      | -      | -                | SPI CLK | -     | -       | -     | -      | -                  | **✓** | SPI Clock                                                                                         |

[<img src="ESP32-DEVKIT-38PINS-pinout.png" width="1000" alt="PINOUT"/>](ESP32-DEVKIT-38PINS-pinout.png)


## ESPHome Configuration
The NODEMCU32 ESP-WROOM-32 can be easily integrated with ESPHome for use in Home Assistant. Here are the basic steps to get started:

1. **Install ESPHome**: Follow the [installation guide](https://esphome.io/guides/installing_esphome.html) on the ESPHome website.
2. **Create a new configuration file**: Create a YAML file for your NODEMCU32 ESP-WROOM-32. Here is an example configuration:

```yaml
esphome:
  name: nodemcu32
  platform: ESP32
  board: nodemcu-32s

wifi:
  ssid: "your-ssid"
  password: "your-password"

# Enable logging
logger:

# Enable Home Assistant API
api:

# Enable Over-The-Air updates
ota:

# Example configuration entry for status LED on GPIO2
light:
  - platform: status_led
    name: "Status LED"
    id: status_led
    pin:
      number: GPIO2
      inverted: true
    restore_mode: ALWAYS_OFF
```

3. **Upload the configuration**: Use the ESPHome command line or the web interface to upload the configuration to your WEMOS D1 Mini ESP32.
4. **Integrate with Home Assistant**: Once the configuration is uploaded, the device will automatically appear in Home Assistant.

For detailed instructions and more configuration options, refer to the [ESPHome documentation](https://esphome.io/).


## Documentation Links

- [Dimensions](pictures/ESP32-DEVKIT-38PINS-dimensions.jpg)
- [Schematic](pdf/ESP32-Core-Board-V2_sch.pdf)
- [ESP32 Datasheet](pdf/esp32_datasheet_en.pdf)

[All boards comparative](../../Docs/comparative-boards.md)