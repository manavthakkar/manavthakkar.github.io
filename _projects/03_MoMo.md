---
name: MoMo - Modular Mobile Robot
tools: [AMR, ROS2, Open Source, nav2]
image: https://manavthakkar.github.io/assets/gifs/momo-with-localization-module.gif
description: Developed ROS2 software stack for the MoMo robot, a modular research platform at the Institut für Technische Logistik - TUHH, enabling hardware integration and autonomous navigation.
#external_url: https://tuhh-itl.github.io/MoMo/
---

# MoMo - Modular Mobile Robot Research Platform

## Overview

MoMo is an open-source autonomous robot designed to serve as a flexible research tool for robotics applications. Currently working on this project under the guidance of [Markus Knitt](https://de.linkedin.com/in/markus-knitt-a67498127) at the **Institut für Technische Logistik (ITL) at TUHH**. 

The primary goal was to design a modular robot that could perform autonomous tasks such as mapping, localization, and navigation using ROS2. Throughout the development process, I worked on the entire system from CAD modeling and simulation to the implementation of navigation and sensor integration. The project is open-source, and the code and documentation are available on [GitHub](https://github.com/TUHH-ITL/MoMo).

![MoMo Robot](https://manavthakkar.github.io/assets/images/momo.jpeg)

*Image source: ITL TUHH Social Media*

<p class="text-center">
{% include elements/button.html link="https://tore.tuhh.de/entities/publication/26e95c56-8320-42a0-91a5-01432206b62c" text="Checkout the published paper here" %}
</p>

## Key Features 

#### 1. **CAD Modeling and URDF Creation**
   - The 3D model of MoMo was created in **SolidWorks** and exported as a URDF using the SolidWorks URDF exporter. This allowed for simulation and visualization in **Gazebo** and **RViz**.
   - The URDF includes joints, links, and sensors, ensuring accurate simulation of the robot’s physical and sensor setup.

### 2. **Autonomous Navigation and Mapping**
   - **Mapping**: I used the **Slam Toolbox** to enable MoMo to create maps of unknown environments in real-time.
   - **Localization**: Implemented localization using the **Nav2 AMCL** package, which provided accurate robot localization in pre-mapped environments.
   - **Navigation Stack**: The full ROS2 **Nav2** stack was implemented to allow for autonomous path planning, dynamic obstacle avoidance, and re-routing.

### 3. **Sensor Fusion**
   - Integrated data from **wheel odometry** and **LiDAR** using the **robot_localization** package, which allowed for improved localization accuracy through sensor fusion.
   - Integrated plugins in Gazebo for simulating the sensors, which included **LiDAR**, **cameras**, and a **depth camera**.

### 4. **Documentation**
   - The documentation for MoMo, including setup instructions, technical details, and animations demonstrating the robot’s capabilities, was created using **MkDocs** and is available [here](https://tuhh-itl.github.io/MoMo/).
   - The animations, created in **Fusion 360**, demonstrate the assembly and modularity of the robot.

MoMo is an open-source project, and all the source code, CAD files, BOM, assembly instructions, URDF files, and documentation are freely available:

- **GitHub Repository**: [MoMo Project on GitHub](https://github.com/TUHH-ITL/MoMo)
- **Documentation Website**: [MoMo Documentation](https://tuhh-itl.github.io/MoMo/)
 
## Technical Stack

- **Programming Languages**: Python, C++
- **Robotics Middleware**: ROS2 (Humble)
- **Simulation Tools**: Gazebo, RViz
- **CAD Software**: SolidWorks, Fusion 360 
- **SLAM and Mapping**: slam_toolbox
- **Navigation**: Nav2
- **Sensor Fusion**: robot_localization
- **Version Control**: Git, GitHub
- **Documentation**: MkDocs

<br>

![ITL-TUHH Team](https://manavthakkar.github.io/assets/images/itl-team.jpg)


ITL Team :)
