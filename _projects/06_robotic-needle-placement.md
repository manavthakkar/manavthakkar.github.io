---
name: Image-Guided Robotic Needle Placement 
tools: [Python, NumPy, ROS]
image: https://manavthakkar.github.io/assets/gifs/robotic-needle-placement.gif
description: Simulating a robotic surgery using a 7-axis Franka-Emika Panda robot arm.
---
# Image-Guided Robotic Needle Placement

## Overview
This project was part of a course on robotics and navigation in medicine, aimed at understanding modern robotic surgeries. The main goal was to accurately detect the position of a tumor in a patient's body and take a sample by inserting a needle using a 7-axis Franka Emika robotic arm, ensuring minimal invasion.

![Robotic Surgery](https://manavthakkar.github.io/assets/images/robotic-surgery.png)

## Project Structure
The project was executed in a team divided into two sub-groups: Vision and Robotics. I was part of the Robotics team.

- **Vision Team**: Responsible for camera calibration using a depth camera and processing the data to provide two 3D poses:
  - The exact location of the tumor.
  - The entry point on the patient's body to ensure minimal invasion.

- **Robotics Team**: Responsible for planning and executing the robotic arm's trajectory to reach the specified locations.

## Technical Details
- **Robotic Arm**: 7-axis Franka Emika
- **Trajectory Planning**: Quintic trajectory planning using fifth-degree polynomials to ensure smooth and precise movements.
- **Simulation Environment**: RViz for initial testing and simulation.
- **Programming Languages and Tools**: ROS (Robot Operating System), Python

## Trajectory Planning
- **Quintic Trajectory Planning**: Implemented quintic polynomials to ensure continuous position, velocity, and acceleration profiles, resulting in smoother movements and reduced abrupt changes in acceleration.
- **Node Development**: Developed a ROS node to move the robotic arm from its current position to the desired pose using quintic trajectory planning.
- **Straight-Line Interpolation**: Created interpolation algorithms to move the needle in a straight line from the entry point to the tumor, minimizing invasion.

## Challenges and Solutions
- **Inverse Kinematics**: Manually calculated the inverse kinematics of the robotic arm without using any frameworks like MoveIt, which provided a deep learning experience in the fundamentals of robotic motion.
- **Simulation to Reality**: Transferring successful simulations to the real robot posed challenges, as some motions that worked in simulation would cause errors in the actual robot. Extensive debugging and testing were required to align the simulation results with real-world performance.

## Learning Outcomes
- Gained hands-on experience in planning and executing robotic trajectories without relying on high-level frameworks.
- Developed skills in manual inverse kinematics calculation.
- Enhanced problem-solving abilities to debug and resolve errors in both simulation and real-world implementations.
- Improved understanding of smooth trajectory planning using quintic polynomials for medical applications.

## Course Context
This project was part of a course called **Robotics and Navigation in Medicine** taken at the [Institute of Medical Technology and Intelligent Systems (MTEC)](https://mtec.et8.tuhh.de/) - TUHH, providing a practical and in-depth understanding of how modern robotic surgeries operate.

This project not only deepened my understanding of robotic surgeries but also honed my skills in trajectory planning, inverse kinematics, and real-world application of robotic systems in the medical field. It was a valuable and enriching learning experience.

<p class="text-center">
{% include elements/button.html link="https://drive.google.com/drive/u/1/folders/1APgcHeqcUnNbrICeB_O92IPUFeoDNwJ5" text="Learn More" %}
</p>