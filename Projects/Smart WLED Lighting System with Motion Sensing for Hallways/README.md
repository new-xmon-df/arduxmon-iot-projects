# Smart WLED Lighting System with Motion Sensing for Hallways 💡🚶‍♂️

Welcome to the Smart WLED Lighting System with Motion Sensing for Hallways project! This project aims to provide intelligent illumination for hallways using motion sensing technology and WLED controllers.

## Description
This project utilizes ESPHome for firmware development and integrates with home automation platforms for easy control and customization. It includes the schematic, PCB design, and firmware files for seamless replication and installation. Get ready to experience enhanced hallway lighting with motion sensing capabilities! 🌟

## Components
- [2 Wemos S2 Mini (ESP32-S2)](../../Boards/WEMOS_S2_MINI/README.md) - [buy](https://www.aliexpress.com/item/1005006157693055.html)
- [PIR Sensor HC-SR501](../../Components/Sensors/Presence/HC-SR501/README.md) - [buy](https://es.aliexpress.com/item/1005006613371075.html)
- [LED WS2812B (30 leds / 1 m.)]() - [buy](https://es.aliexpress.com/item/1005004289391906.html)

## Files Included
- [`hallway_sensor.yaml`](firmware/hallway_sensor.yaml): ESPHome firmware configuration file.
    - [`wemos-s2-mini.yaml)`](firmware/boards/wemos-s2-mini.yaml)
    - [`wifi_domotica.yaml`](firmware/common/wifi_domotica.yaml)
- [`blueprint`](home_assistant/blueprints/motion_light_wled.yaml): create your automation with the blueprint
- [`schematic.pdf`](): pending
- [`LICENSE`](LICENSE): Creative Commons Attribution-ShareAlike 4.0 International License

## Installation WLED
1. ...

## Installation PIR Sensor
1. Flash the ESPHome firmware onto the Wemos S2 Mini using the provided configuration [file](firmware/hallway_sensor.yaml).
2. Set up the Home Assistant automation using the provided blueprint [file](home_assistant/blueprints/motion_light_wled.yaml).

## Usage

## Screenshots

### Home Assistant Dashboard

## License
This project is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](LICENSE).

Feel free to contribute, modify, and share!

