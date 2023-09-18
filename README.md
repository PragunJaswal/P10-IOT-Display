# IoT Display Control with Arduino

![IoT Display](https://i0.wp.com/roboticsdna.in/wp-content/uploads/2021/05/p10-3216-red-led-display.jpg?fit=1000%2C1000&ssl=1)

This project demonstrates IoT display made by NodeMCU ESP8266 board and 4* P10 LED panel. It allows you to toggle between "News" and "Notice" modes and display relevant information.

## Overview

This project comprises Arduino code for controlling the P10 LED panel and fetching data from external sources. The display can scroll text messages, show the current date and time, and fetch news or notices based on user selection.

## Features

- Display text messages on a P10 LED panel.
- Display the time from WORLDAPI
- Toggle between "News" and "Notice" modes.
- Fetch and display news or notices from external sources.
- Automatic switch to the current date and time display.
- Handle network connectivity issues gracefully.

## Hardware Setup

1. Connect your P10 LED panel to the Arduino board following the pinout and wiring instructions.

2. Upload the provided Arduino code to your Arduino board.

3. Power up the hardware and ensure a stable network connection.

## Usage

1. Upon startup, the display will show a scrolling welcome message.

2. You can toggle between "News" and "Notice" modes using the web interface or by modifying the Arduino code.

3. In "News" mode, the display will fetch and scroll top news headlines.

4. In "Notice" mode, the display will show notices fetched from an external source.

5. After a period of time, the display will switch back to the current date and time display.

## Web Interface

You can interact with the IoT display using a web interface. The web interface allows you to control the display mode and send notices to be displayed.

Access the web interface by opening a web browser and entering the IP address of the Arduino board.
## APIs Used

### 1. News API
- **Description:** Fetches top news headlines.
- **Endpoint:** `https://news-api-vaqm.onrender.com/news-top`

### 2. Notice API
- **Description:** Retrieves notices for display.
- **Endpoint:** `https://news-api-vaqm.onrender.com/get/notice`

### 3. Toggle API
- **Description:** Controls the display mode (News/Notice).
- **Endpoint:** `https://news-api-vaqm.onrender.com/toggle`

## Dependencies

- [ESP8266WebServer](https://github.com/esp8266/ESPWebServer) - Used to create the web interface.
- [DMDESP](https://github.com/FrankBoesing/DMXSerial2) - Library for controlling P10 LED panels.
- [ArduinoJson](https://github.com/bblanchon/ArduinoJson) - Used to parse JSON data from external sources.

## Troubleshooting

If you encounter issues with the display or connectivity, consider the following:

- Check the hardware connections and wiring.
- Ensure a stable Wi-Fi connection.
- Inspect the Arduino serial monitor for error messages.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to [Sahil Bhardwaj] for the web interface.
- Special thanks to the Arduino and open-source community for their contributions.

## Author
[Pragun jaswal]


Feel free to update the code as per requirement..
