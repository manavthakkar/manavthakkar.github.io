---
name: IoT Sports Scoreboard
tools: [Microcontroller, IoT, ESP32]
image: https://manavthakkar.github.io/assets/images/iot-sports-scoreboard.png
description: Access the real-time game score on a display using the power of IoT! 
---
# IoT Sports Scoreboard

This project showcases the integration of Internet of Things (IoT) technology with live sports data. Using an ESP32 microcontroller, the scoreboard continuously fetches cricket match data and displays it on an LCD screen.

## Features

- **Real-Time Data Fetching**: The scoreboard fetches live data from the Cricbuzz website via a custom API made with ThingSpeak.
- **ESP32 Microcontroller**: Utilizes the popular ESP32 board for processing and connectivity.
- **LCD Display**: Displays the fetched data on a 16×2 I2C LCD display for real-time updates.

## Technical Details

- **Microcontroller**: ESP32
- **API**: Custom API created using ThingSpeak to interface with Cricbuzz
- **Display**: 16×2 I2C LCD
- **Programming Languages**: C/C++ (Arduino IDE)

## Project Workflow

1. **Data Collection**: The Cricbuzz website's API is used to fetch live cricket match data.
2. **API Integration**: A custom API was created using ThingSpeak to streamline data fetching and processing.
3. **Data Processing**: The ESP32 processes the incoming data and prepares it for display.
4. **Display**: The processed data is displayed on the 16×2 I2C LCD, providing real-time updates.

## Learning Outcomes

- Gained practical experience in IoT and microcontroller programming.
- Developed skills in API creation, data processing, and hardware integration.
- Explored the potential of physical interactions in enhancing engagement and interactivity.

## Future Enhancements

- Expand physical interaction capabilities with additional sensors and actuators.
- Implement customizable alert systems for specific events or match situations.
- Explore integration with other IoT devices for a comprehensive sports viewing experience.

<p class="text-center">
{% include elements/button.html link="https://www.linkedin.com/posts/manavt2000_iot-internetofthings-esp32-ugcPost-6792124845103583232-5Qhq/" text="Learn More" %}
</p>