---
name: Autonomous Navigation with Elevation Mapping
tools: [C++, ROS, Quadruped]
image: https://manavthakkar.github.io/assets/images/obstacles.png
description: Built a system for quadruped robots to navigate around obstacles using real-time elevation maps.
---

## Autonomous Navigation with Elevation Mapping for Quadruped Robots

## Overview

This project focuses on integrating **[2.5D elevation mapping](https://github.com/ANYbotics/elevation_mapping)** into the motion planning framework of quadruped robots to enhance their ability to traverse uneven terrains. Conducted under the guidance of [Aditya Tandon, M.Sc.](https://de.linkedin.com/in/tandon-aditya), this project was completed at the **Institute of Digital and Autonomous Construction (IDAC), Hamburg University of Technology**.


<div style="display: flex; justify-content: center; align-items: center; gap: 20px;">
  <div>
    <img src="../assets/gifs/obstacle.gif" alt="GIF 1" style="max-width: 100%; height: auto;">
    <p style="text-align: center;"><em>Without elevation mapping</em></p>
  </div>
  <div>
    <img src="../assets/gifs/avoid-obstacle.gif" alt="GIF 2" style="max-width: 100%; height: auto;">
    <p style="text-align: center;"><em>With elevation mapping</em></p>
  </div>
</div>


The project utilized the **IDOG (Intelligent Documentation Gadget)** i.e. Unitree A1 quadruped robot as the test platform and focused on real-time integration of elevation data with path planning to improve autonomous navigation in dynamic and complex environments.

---

{% include elements/video.html id="CFtqexe72H4" %}

---

## Key Features

### 1. **Elevation Mapping**
- Implemented a robot-centric **2.5D elevation mapping** system using the open-source `elevation_mapping` ROS package.
- Dynamically updated elevation maps in real-time based on terrain height and sensor input.
- Used **Intel RealSense D435i** depth camera for capturing point cloud data.

### 2. **Path Planning Integration**
- Integrated the elevation map into the ROS `costmap_2d` framework by adding a custom **elevation layer**.
- Enabled real-time obstacle avoidance and dynamic path re-planning by incorporating height constraints into the navigation stack.

### 3. **Validation and Testing**
- Validated the system in a controlled indoor environment with various obstacles and terrain variations.
- Demonstrated successful obstacle detection and navigation through uneven terrains, outperforming traditional 2D mapping methods.

### 4. **Hardware Setup**
- Primary computation was performed on **Jetson Xavier NX**, with elevation mapping offloaded to an **Intel NUC** running ROS Noetic.
- Fully integrated **Intel RealSense D435i** for depth sensing and LiDAR for obstacle detection.



## Technical Stack

- **Programming Languages**: C++
- **Robotics Middleware**: ROS Melodic/Noetic
- **Mapping Framework**: [elevation_mapping](https://github.com/ANYbotics/elevation_mapping)
- **Costmap Integration**: [costmap_2d](http://wiki.ros.org/costmap_2d)
- **Sensor Fusion**: Depth Camera (Intel RealSense D435i), LiDAR
- **Visualization**: RViz
- **Computing Units**: Jetson Xavier NX, Intel NUC


## Results

- Improved navigation accuracy by dynamically integrating elevation data into path planning.
- Enabled the robot to safely traverse obstacles undetectable by traditional sensors, such as LiDAR.
- Successfully demonstrated autonomous navigation in a simulated construction site.


The presentation for this project can be found [here](https://docs.google.com/presentation/d/1ZUIUlANvL4nHu4aaX5m-RTa3UdeAc5lBVQsdEUl_fEc/edit?usp=sharing)
