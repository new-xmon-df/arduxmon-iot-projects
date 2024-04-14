# LDR 5528 Sensor

The LDR 5528 sensor is a light-dependent resistor capable of detecting changes in light intensity. Here's a detailed
overview of the LDR 5528 sensor and its integration into your IoT projects:

[<img src="pictures/LDR-5528.png" width="400" alt="LDR-552"/>](pictures/LDR-5528.png)

## Description

The LDR 5528 sensor is commonly used for light detection and ambient light monitoring in various applications, including
automatic lighting systems, brightness control, and security systems.

## Technical Specifications

- Sensor Type: Light Dependent Resistor (LDR)
- Operating Voltage: Typically 3.3V or 5V

## Features

- Responsive to changes in light intensity for accurate light detection.
- Compact and easy-to-install design for versatile applications.
- Analog output for interfacing with microcontrollers and analog-to-digital converters (ADCs).

## Integration

Integrating the LDR 5528 sensor into your project is simple. Connect one terminal of the LDR to the microcontroller's
analog input pin and the other terminal to ground. Additionally, connect a pull-down resistor, typically with a value of
around 10k ohms, between the analog input pin and ground to ensure stable readings. You can then read the analog voltage
output from the sensor and interpret it as a measure of light intensity.

### Additional Information

There are modules that already incorporate all the necessary circuitry for the use of the photoresistor, such as the
**KY-018**.

## Schema


Personally, I create a module like the KY-018, I also share the schema.

[<img src="schemas/LDR-5528-Pinout.png" width="500" alt="Pinout"/>](schemas/LDR-5528-Pinout.png)

This is the schema with which the LDR must be integrated into our projects.

[<img src="schemas/ldr-5528-schema.png" width="500" alt="Schema"/>](schemas/ldr-5528-schema.png)


## Projects
Explore examples of projects incorporating the BME680 sensor for inspiration and guidance on how to utilize its capabilities in your own projects.

- [**Living room sensors**](../../../../Projects/Living%20room%20sensors/README.md): Multi-sensor system for living room.
- [**Plant Irrigation Control**](../../../../Projects/Plant%20irrigation%20control/README.md): This project aims to control the soil moisture of multiple plants.

## Documentation Links

- [Datasheet](pdf/SEN-09088.pdf)
