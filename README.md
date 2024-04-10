# Welcome to Arduxmon IoT projects!  💀🌟

Hey there, tech enthusiasts! I'm Arduxmon, a passionate developer and graphic designer with an insatiable love for IoT projects. In this space, I share my craziest and coolest creations so we can all learn, experiment, and improve together. 💡🛠️

### What will you find here?

1. **ESPHome Code**: Dive into the world of microcontroller programming with a variety of ESPHome codes. From temperature sensors to smart lighting systems, you'll find it all here!

2. **Home Assistant Configurations**: Make your home smarter with our Home Assistant configurations. Control lights, thermostats, cameras, and more, all from the comfort of your smartphone!

3. **Electronic Schematics**: Discover how the pieces are connected with our detailed electronic schematics. From the basics to more advanced projects, we have the blueprints you need!

4. **PCB Designs and Gerber Files**: Take your projects to the next level with our PCB designs and ready-to-produce Gerber files. Bring your ideas to life!

### Projects in the Repository

- [**Living room sensors**](Projects/Living%20room%20sensors/README.md): Multi-sensor system for living room.
- [**Plant Irrigation Control System**](Projects/Plant%20irrigation%20control/README.md) _incomplete_: An automated irrigation system for plants.

### ESP Boards Used in the Project:
In this section, we will delve into the heart of my IoT projects: the ESP boards. These powerful microcontrollers have been instrumental in creating smart and connected solutions.

1. **ESP32**: 
is a versatile and powerful board that offers integrated WiFi and Bluetooth connectivity. Its dual-core processor and wide range of peripherals make it an ideal choice for projects requiring high performance and wireless communication.
   - **Technical details**:
     - Processor: Dual-core Xtensa LX6 at 240 MHz
     - Connectivity: WiFi 802.11 b/g/n, Bluetooth v4.2 BR/EDR and BLE
     - Interfaces: GPIO, SPI, I2C, UART, PWM, ADC, DAC, etc.
     - Memory: 520 KB SRAM, 4 MB Flash
2. **ESP8266**: 
is another popular and affordable board known for its integrated WiFi connectivity. Although it has fewer resources than the ESP32, it is perfect for simpler projects requiring internet connection and remote control.
   - **Technical details**:
     - Processor: Single-core Xtensa LX106 at 80 MHz
     - Connectivity: WiFi 802.11 b/g/n
     - Interfaces: GPIO, SPI, I2C, UART, PWM, ADC
     - Memory: 80 KB RAM, 1 MB Flash
3. **Uses in my Projects**:
   Both ESP boards have been used in various projects to control sensors, send data to the cloud, receive remote commands, and automate tasks. Their ease of programming, low power consumption, and active development community make them indispensable tools for implementing IoT solutions. Throughout this section, I will explore in detail how we have maximized the capabilities of these boards to create intelligent and connected systems that meet the needs of our users.

    In this section, I will detail the specific boards that I have used in my IoT projects. Each of these boards has been selected for its particular features and capabilities to meet the requirements of each project.

    - **[WEMOS S2 MINI:](Boards/WEMOS_S2_MINI/README.md)**
      This board uses the **ESP32-S2**, offering an alternative with higher performance and advanced features such as native USB and increased RAM and Flash compared to the ESP8266.

   - **[WEMOS D1 MINI](Boards/WEMOS_D1_MINI/README.md)** v1, v2, v3, and v4:
      These compact boards based on the **ESP8266** are ideal for projects that require WiFi connectivity and a small footprint. Versions v1, v2, v3, and v4 offer progressive improvements in performance and features.

   - **[LOLIN32 Lite:](Boards/LOLIN32_Lite/README.md)**
     The LOLIN32 Lite is an **ESP32**-based board that strikes a balance between performance and power consumption. It's ideal for projects requiring WiFi and Bluetooth connectivity, as well as processing power.

   - **ESP32-DevKitC 38 pins:**
     This ESP32-based development kit offers a wide range of interfaces and peripherals, including GPIO, SPI, I2C, UART, PWM, and more, making it a versatile choice for complex projects.

   - **WEMOS D1 UNO R3:**
   The WEMOS D1 UNO R3 combines compatibility with Arduino UNO R3 with the capabilities of ESP8266, making it perfect for projects that need a familiar Arduino interface and WiFi connectivity.

   - **ESP32-C3 Supermini:**
   The ESP32-C3 Supermini is a compact version of the ESP32-C3 that provides WiFi and Bluetooth LE connectivity. Its small size makes it ideal for applications where space is limited.

### Components Used in my Projects:
In this section, I categorize the components utilized in my projects according to their type. Each component type is accompanied by a general description, and each specific component is linked to its respective documentation.

1. **Displays**: are essential components in many of my IoT projects, providing visual feedback and information display to users. Explore the diverse range of displays I've integrated:

    - [SH1116](Components/Displays/SH1106/README.md): The SH1106 display is a popular choice among hobbyists and professionals alike, offering high contrast and excellent visibility in various lighting conditions. Here's what you need to know about integrating the SH1106 display into your IoT projects:

2. **Sensors**:
   Sensors play a crucial role in gathering environmental data and enabling smart functionalities in my projects. Explore the different types of sensors I've integrated, each serving a unique purpose:

   - **Environmental**:
     - [BME680](Components/Sensors/Environmental/BME680/README.md): The BME680 sensor is a versatile environmental sensor capable of measuring temperature, humidity, pressure, and gas levels.
     - BMP280: *Documentation pending*
     
   - **Distance**:
     - [HC-SR04](Components/Sensors/Distance/HC-SR04/README.md): The HC-SR04 is an ultrasonic distance sensor capable of measuring distance accurately using ultrasonic waves.

   - **Light**:
     - [LDR 5528](Components/Sensors/Light/LDR_5528/README.md): The LDR 5528 is a light-dependent resistor that changes resistance based on the intensity of light falling on its surface.

   - **Magnetic**:
     - MC-38: *Documentation pending*
     - [A3144E](Components/Sensors/Magnetic/A3144E/README.md): A3144E Hall Effect sensor: versatile for proximity, speed, and current sensing.

   - **Presence**:
     - [LD2410c](Components/Sensors/Presence/LD2410c/README.md): The LD2410C sensor by Hilink Electronics utilizes 24GHz FMCW technology for highly sensitive human presence detection, including precise motion and stationary state detection and distance calculation. It boasts compact dimensions of 22mm x 16mm and features a standard 2.54mm pin spacing
     - [LD2410b](Components/Sensors/Presence/LD2410b/README.md): The LD2410b sensor by Hilink Electronics detects human presence with high sensitivity using FMCW at 24GHz, enabling precise detection of motion and stationary states, along with distance calculation.
     - [HC-SR501](Components/Sensors/Presence/HC-SR501/README.md): The HC-SR501 PIR Motion Detector is based on infrared technology, featuring an automatic control module designed with a high-sensitivity.
     - LD2411: *Documentation pending*

   - **Soil Moisture**:
     - [Capacitive Soil Moisture](Components/Sensors/Soil%20Moisture/Capacitive%20Soil%20Moisture/README.md): Capacitive soil moisture sensor measures moisture, differing from resistive sensors.

   - **Temperature**:
     - DS18B20: *Documentation pending*
     
   - **Vibration**:
     - [Piezoelectric Vibration & Knock Sensor Module](Components/Sensors/Vibration/SSR1072-Piezo-Vibration-Sensor/README.md): The Piezoelectric Vibration & Knock Sensor Module offers versatility in motion detection, with analog/digital outputs and sensitivity adjustment for seamless project integration.

### How can you contribute?

I love the idea of building a collaborative community! If you have improvements, corrections, or new projects to add, feel free to make a contribution! Simply fork the repository, make your changes, and send a pull request.

### Ready to get started?

Awesome! Check out my projects, clone the repository, and start exploring. If you have any questions, suggestions, or just want to chat about IoT, feel free to contact me!

Thanks for being part of this exciting IoT community!

