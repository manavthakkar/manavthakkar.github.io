---
name: Hand Gesture Based Control 
tools: [Python, Arduino, OpenCV]
image: https://manavthakkar.github.io/assets/images/hand-gesture.png
description: Developed hand gesture control systems using computer vision, applying them to various interactive applications.
---
# Hand Gesture Based Control

During an internship, I delved into computer vision, particularly intrigued by OpenCV and Mediapipe libraries. This led me to create a project aimed at detecting hand gestures and utilizing them to control LEDs. Using OpenCV and Mediapipe, the system accurately identifies hand landmarks, which serve as the foundation for gesture detection. By analyzing the position of these landmarks, the system determines the number of raised fingers, thereby identifying specific gestures.

<p class="text-center">
{% include elements/button.html link="https://www.linkedin.com/feed/update/urn:li:activity:6822224336858955776/" text="Working video" %}
</p>

![Hand Gesture Control](https://manavthakkar.github.io/assets/images/hand-gesture-control.jpg)

*Image source: 8th Wall / Arian Badri*

## Technology Stack

- OpenCV
- Mediapipe
- Python
- Arduino

## Functionality

The system operates through a Python script that processes hand landmark data and translates it into gestures. For instance, raising two fingers might signify a specific gesture, represented by a predefined binary array. This data is then transmitted serially from Python to an Arduino board, which interprets the gesture and controls the LEDs accordingly.

## Challenges

Integrating software and hardware components posed a significant challenge, especially establishing communication between Python and Arduino. Despite being relatively new to programming at the time, overcoming this hurdle provided invaluable learning experiences.

## Future Enhancements

With further development, it can be extended to control various devices and appliances, offering a versatile and intuitive interface for interaction.

## Recognition

This project received second prize in the All India Automation Contest 2021, earning a prize money of 25,000 INR. [(announcement video)](https://www.linkedin.com/posts/manavt2000_automation-ai-contest-activity-6882935661393977344-V3ps?utm_source=share&utm_medium=member_desktop)


More details about the project can be found [here](https://circuitdigest.com/microcontroller-projects/gesture-based-intelligent-appliance-control).

<br>

## Hand Gesture Controlled Chrome Dino Game

![Chrome Dino Game](https://manavthakkar.github.io/assets/images/chrome-dino.png)

After sharing my previous hand gesture project, I received a suggestion to create something similar for the Chrome Dino game. For this project, I once again used OpenCV and Mediapipe libraries in conjunction with Python.

The system detects hand landmarks, specifically focusing on the first finger tip and the tip of the thumb. If the distance between these two points exceeds a certain threshold, the Python script simulates a space bar press, causing the Dino to jump in the game. This simple yet effective method allows for intuitive control of the game through hand gestures.

One of the key challenges was to prevent multiple detections for the same gesture, which could lead to erratic game behavior. Additionally, determining the appropriate threshold values was tricky, as they vary depending on the distance of the hand from the camera. Through trial and error, I was able to find a balance that provided a smooth gaming experience.

<p class="text-center">
{% include elements/button.html link="https://www.linkedin.com/feed/update/urn:li:activity:6824778804926418944/" text="Working video" %}
</p>