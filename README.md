# Welcome to Arduxmon IoT Projects! 💀🌟

Hey there, tech enthusiasts! I'm Arduxmon, a passionate developer and graphic designer with an insatiable love for IoT
projects. In this space, I share my craziest and coolest creations, so we can all learn, experiment, and improve
together. 💡🛠️

### What will you find here?

1. **ESPHome Code**: Dive into the world of microcontroller programming with a variety of ESPHome codes. From
   temperature sensors to smart lighting systems, you'll find it all here!

2. **Home Assistant Configurations**: Make your home smarter with our Home Assistant configurations. Control lights,
   thermostats, cameras, and more, all from the comfort of your smartphone!

3. **Electronic Schematics**: Discover how the pieces are connected with our detailed electronic schematics. From the
   basics to more advanced projects, we have the blueprints you need!

4. **PCB Designs and Gerber Files**: Take your projects to the next level with our PCB designs and ready-to-produce
   Gerber files. Bring your ideas to life!

### Projects in the Repository

- [**Living Room Sensors**](Projects/Living%20room%20sensors/README.md): Multi-sensor system for the living room.
- [**Plant Irrigation Control System**](Projects/Plant%20irrigation%20control/README.md) _(incomplete)_: An automated
  irrigation system for plants.

### ESP Boards Used in the Projects

In this section, we will delve into the heart of my IoT projects: the ESP boards. These powerful microcontrollers have
been instrumental in creating smart and connected solutions.

1. **ESP32**:
   The ESP32 is a versatile and powerful board that offers integrated Wi-Fi and Bluetooth connectivity. Its dual-core
   processor and wide range of peripherals make it an ideal choice for projects requiring high performance and wireless
   communication.
    - **Technical Details**:
        - Processor: Dual-core Xtensa LX6 at 240 MHz
        - Connectivity: Wi-Fi 802.11 b/g/n, Bluetooth v4.2 BR/EDR and BLE
        - Interfaces: GPIO, SPI, I2C, UART, PWM, ADC, DAC, etc.
        - Memory: 520 KB SRAM, 4 MB Flash
2. **ESP8266**:
   The ESP8266 is another popular and affordable board known for its integrated Wi-Fi connectivity. Although it has
   fewer resources than the ESP32, it is perfect for simpler projects requiring an internet connection and remote
   control.
    - **Technical Details**:
        - Processor: Single-core Xtensa LX106 at 80 MHz
        - Connectivity: Wi-Fi 802.11 b/g/n
        - Interfaces: GPIO, SPI, I2C, UART, PWM, ADC
        - Memory: 80 KB RAM, 1 MB Flash
3. **Uses in my Projects**:
   Both ESP boards have been used in various projects to control sensors, send data to the cloud, receive remote
   commands, and automate tasks. Their ease of programming, low power consumption, and active development community make
   them indispensable tools for implementing IoT solutions. Throughout this section, I will explore in detail how we
   have maximized the capabilities of these boards to create intelligent and connected systems that meet the needs of
   our users.

   In this section, I will detail the specific boards that I have used in my IoT projects. Each of these boards has been
   selected for its particular features and capabilities to meet the requirements of each project.
    - **[ESP32-C3 Supermini](Boards/ESP32_C3_SUPERMINI/README.md)**:
      The ESP32-C3 Supermini is a compact version of the ESP32-C3 that provides Wi-Fi and Bluetooth LE connectivity. Its
      small size makes it ideal for applications where space is
      limited. [ESP32-C3 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32c3/hw-reference/index.html).
    - **[ESP32-C3 ZERO](Boards/ESP32_C3_ZERO/README.md)**:
      The ESP32-C3-ZERO is a versatile board offering Wi-Fi and Bluetooth LE connectivity, designed for efficient
      performance with a reduced pin count. Its compact form factor is suitable for various IoT
      applications. [ESP32-C3 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32c3/hw-reference/index.html).
    - **[ESP32-DevKitC 38 Pins](Boards/ESP32-DEVKIT-38PINS/README.md)**:
      This ESP32-based development kit offers a wide range of interfaces and peripherals, including GPIO, SPI, I2C,
      UART, PWM, and more, making it a versatile choice for complex
      projects. [ESP32 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32/hw-reference/index.html).
    - **[LOLIN32 Lite](Boards/LOLIN32_Lite/README.md)**:
      The LOLIN32 Lite is an ESP32-based board that strikes a balance between performance and power consumption. It's
      ideal for projects requiring Wi-Fi and Bluetooth connectivity, as well as processing
      power. [ESP32 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32/hw-reference/index.html).
    - **[WEMOS D1 MINI](Boards/WEMOS_D1_MINI/README.md)** v1, v2, v3, and v4:
      These compact boards based on the ESP8266 are ideal for projects that require Wi-Fi connectivity and a small
      footprint. Versions v1, v2, v3, and v4 offer progressive improvements in performance and features.
    - **[WEMOS D1 MINI ESP32](Boards/WEMOS_D1_MINI_ESP32/README.md)**:
      The WEMOS D1 MINI ESP32 is a compact board that offers Wi-Fi and Bluetooth LE connectivity. It's ideal for
      projects that require a small size without sacrificing performance and connectivity capabilities. ESP32 Hardware
      Reference. [ESP32 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32/hw-reference/index.html).
    - **[WEMOS S2 MINI](Boards/WEMOS_S2_MINI/README.md)**:
      This board uses the ESP32-S2, offering an alternative with higher performance and advanced features such as
      native
      USB and increased RAM and Flash compared to the
      ESP8266. [ESP32-S2 Hardware Reference](https://docs.espressif.com/projects/esp-idf/en/v4.3/esp32s2/hw-reference/index.html).
    - **WEMOS D1 UNO R3**:
      The WEMOS D1 UNO R3 combines compatibility with Arduino UNO R3 with the capabilities of ESP8266, making it
      perfect
      for projects that need a familiar Arduino interface and Wi-Fi connectivity.

To help you choose the most suitable development board for your projects, I have created a comprehensive comparison
table of various ESP32 and WEMOS boards. This table includes detailed information on processors, memory capacities,
performance, dimensions, and specific features of each board.

You can view and download the full comparative document [here](Docs/comparative-boards.md).

### Components Used in My Projects

In this section, I categorize the components utilized in my projects according to their type. Each component type is
accompanied by a general description, and each specific component is linked to its respective documentation.

1. **Displays**: Displays are essential components in many of my IoT projects, providing visual feedback and information
   display to users. Explore the diverse range of displays I've integrated:
    - [SH1106](Components/Displays/SH1106/README.md): The SH1106 display is a popular choice among hobbyists and
      professionals alike, offering high contrast and excellent visibility in various lighting conditions. 

2. **Transistors**:
   - **MOSFETs**:
      - **NPN**:
         - [AO3400A](Components/Transistors/Mosfets/NPN/AO3400A/README.md):
           The AO3400A is a versatile N-channel MOSFET with low on-resistance and fast switching capabilities. It is
           suitable for applications requiring efficient power management and high-speed switching, commonly used in
           power supplies and motor control circuits.

3. **Power Management**:
   - **Step-Down (Buck) Converters**:
      - [MP1584EN](Components/Power%20Management/Step-Down%20Converters/MP1584EN/README.md):
        The MP1584EN is a high-efficiency, step-down DC-DC converter that provides up to 3A output current. It is
        ideal for applications requiring compact size and high performance, such as battery-powered devices and
        portable electronics.
      - [DC-DC 12V to 3.3V 5V Buck Converter Module (T89)](Components/Power%20Management/Step-Down%20Converters/T89-DC-DC%2012V%20to%203.3V-5V/README.md):
        This module efficiently steps down 12V DC input to regulated 3.3V and 5V outputs. It is perfect for powering
        microcontrollers, sensors, and other electronics requiring stable lower voltages from a 12V source.
   - **Step-Up (Boost) Converters**:
      - [MT3608](Components/Power%20Management/Step-Up%20Converters/MT3608/README.md):
        The MT3608 is a high-efficiency, step-up DC-DC converter capable of boosting input voltages as low as 2V to
        output voltages up to 28V. It is commonly used in projects needing voltage conversion for sensors, displays,
        and other components.


1. **Sensors**:
   Sensors play a crucial role in gathering environmental data and enabling smart functionalities in my projects.
   Explore the different types of sensors I've integrated, each serving a unique purpose:

    - **Distance**:
        - [HC-SR04](Components/Sensors/Distance/HC-SR04/README.md): The HC-SR04 is an ultrasonic distance sensor capable
          of measuring distance accurately using ultrasonic waves.

    - **Environmental**:
        - [AHT20 + BME280 Module](Components/Sensors/Environmental/CJMCU-680/README.md):  The AHT20 + BMP280 module combines temperature, humidity, and pressure sensing capabilities into a single device, offering a comprehensive solution for environmental monitoring in IoT projects.
        - [CJMCU-680 Module (BME680 Sensor)](Components/Sensors/Environmental/CJMCU-680/README.md): The BME680 sensor is a versatile environmental sensor capable of measuring temperature, humidity, pressure, and gas levels. This is the low-cost CJMCU-680 Module.
        - BMP280: *Documentation pending*

    - **Light**:
        - [LDR 5528](Components/Sensors/Light/LDR_5528/README.md): The LDR 5528 is a light-dependent resistor that
          changes resistance based on the intensity of light falling on its surface.

    - **Magnetic**:
        - [A3144E](Components/Sensors/Magnetic/A3144E/README.md): A3144E Hall Effect sensor: versatile for proximity,
          speed, and current sensing.
        - [MC-38](Components/Sensors/Magnetic/MC-38/README.md): reliable wired door/window sensor with a magnetic
          switch. It detects the opening and closing of doors and windows, making it ideal for security systems. It
          features a normally closed (NC) circuit that opens when the magnet is moved away.

    - **Presence**:
        - [HC-SR501](Components/Sensors/Presence/HC-SR501/README.md): The HC-SR501 PIR Motion Detector is based on
          infrared technology, featuring an automatic control module designed with high sensitivity.
        - [LD2410b](Components/Sensors/Presence/LD2410b/README.md): The LD2410b sensor by Hilink Electronics detects
          human presence with high sensitivity using FMCW at 24GHz, enabling precise detection of motion and stationary
          states, along with distance calculation.
        - [LD2410c](Components/Sensors/Presence/LD2410c/README.md): The LD2410C sensor by Hilink Electronics utilizes
          24GHz FMCW technology for highly sensitive human presence detection, including precise motion and stationary
          state detection and distance calculation. It boasts compact dimensions of 22mm x 16mm and features a standard
          2.54mm pin spacing.
        - LD2411: *Documentation pending*

    - **Soil Moisture**:
        - [Capacitive Soil Moisture](Components/Sensors/Soil%20Moisture/Capacitive%20Soil%20Moisture/README.md):
          Capacitive soil moisture sensor measures moisture, differing from resistive sensors.

    - **Temperature**:
        - [DS18B20](Components/Sensors/Temperature/DS18B20/README.md): digital temperature sensor offering 9-bit to
          12-bit Celsius temperature measurements with high accuracy. It uses a 1-Wire interface, making it easy to
          connect multiple sensors on the same data line.

    - **Vibration**:
        - [Piezoelectric Vibration & Knock Sensor Module](Components/Sensors/Vibration/SSR1072-Piezo-Vibration-Sensor/README.md):
          The Piezoelectric Vibration & Knock Sensor Module offers versatility in motion detection, with analog/digital
          outputs and sensitivity adjustment for seamless project integration.

### How can you contribute?

I love the idea of building a collaborative community! If you have improvements, corrections, or new projects to add,
feel free to make a contribution! Simply fork the repository, make your changes, and send a pull request.

### Ready to get started?

Awesome! Check out my projects, clone the repository, and start exploring. If you have any questions, suggestions, or
just want to chat about IoT, feel free to contact me!

Thanks for being part of this exciting IoT community!

