---
name: ROS Web GUI 
tools: [ROS, GUI, Quadruped]
image: https://manavthakkar.github.io/assets/images/web-gui.png
description: An app designed to help users track their squat exercises . It offers real-time feedback and voice notifications, making it a convenient tool for monitoring squat workouts.
---
# Web-Based GUI Application for Controlling a ROS-Based Quadruped Robot

## Overview

This project is a web-based GUI application designed to give users intuitive control over a quadruped robot. It features real-time video streaming from the robot’s camera and a human-following mode.

![ROS Web GUI](https://manavthakkar.github.io/assets/images/web-gui.png)

## Key Features

1. **Interactive User Interface:**
   - The user-friendly web-based GUI lets you control the robot with directional buttons and a joystick. There are also buttons for predefined actions like making the robot greet or do pushups.
   - You can watch the robot’s live video feed right in the GUI, giving you a real-time view of what the robot sees.

2. **Dual Control Modes:**
   - **Teleoperation Mode:** Take direct control of the robot’s movements with the directional buttons and joystick.
   - **Human-Following Mode:** Let the robot follow you! Using the MediaPipe library from Google, the robot detects human body landmarks and follows a point on the abdomen to move in sync with you.

3. **Technologies Behind the Scenes:**
   - **Frontend:** Built with HTML, CSS, and JavaScript for a responsive and engaging user experience.
   - **Backend:** Utilizes ROS and Rosbridge to handle communication between the GUI and the robot.
   - **Video Streaming:** The live feed from the robot's camera is published on a ROS topic and integrated into the GUI.

4. **Overcoming Challenges:**
   - **Latency Issues:** We faced some latency problems due to the university’s Wi-Fi network, which affected real-time performance. As a workaround, we used a mobile hotspot to connect all systems on the same network, reducing lag and improving responsiveness.

5. **Course Project Insight:**
   - This project was part of a university course called Construction Robotics. We wrote a paper about it, detailing our approach and findings. You can check it out [here](https://drive.google.com/file/d/1J3n438PW5EqMj7WWqf7FyHSNZ-YNkqSv/view?usp=drive_link).

## Technical Details

- **Frontend Development:**
  - The GUI is designed with HTML, CSS, and JavaScript, providing an interactive and visually appealing interface.
  - Real-time video streaming from the robot’s camera is integrated directly into the GUI for immediate feedback.

- **Backend Integration:**
  - Rosbridge is used to facilitate communication between the web-based GUI and the ROS backend.
  - ROS topics handle the control commands and video data streaming, ensuring smooth operation.

- **Human-Following Feature:**
  - Using Google’s MediaPipe library, the robot detects and tracks human body landmarks.
  - The robot follows a designated point on the abdomen, which directs its movement.

  ![Control Logic](https://manavthakkar.github.io/assets/images/rectangle.jpg)

  Github repository for this project can be found [here](https://github.com/manavthakkar/construction-robotics-TUHH).

<p class="text-center">
{% include elements/button.html link="https://www.linkedin.com/feed/update/urn:li:activity:7162078663511896064/" text="Learn More" %}
</p>