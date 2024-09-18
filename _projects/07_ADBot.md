---
name: ADBot
tools: [ROS, Navigation, AMR]
image: https://manavthakkar.github.io/assets/gifs/adbot.gif
description: An autonomous delivery robot designed for indoor environments, capable of securely delivering goods while avoiding obstacles.
---
## ADBot: Autonomous Delivery Robot

Our final year project aimed to create an indoor autonomous delivery robot designed to assist in delivery operations within environments such as offices and hospitals, ensuring the safety and security of delivered items. The robot uses the ROS (Robot Operating System) navigation stack, allowing users to select the delivery location on a map. The robot autonomously navigates to the specified location, avoiding both static and dynamic obstacles in real-time.

![ADBot drawing](https://manavthakkar.github.io/assets/images/adbot-drawing.jpeg)

Upon reaching the destination, the recipient must show a unique QR code to authenticate and unlock the robot's door via a servo mechanism. If the QR code is incorrect, the robot emits a beeping sound to indicate unauthorized access. Additionally, the robot streams real-time video feed, enabling the sender to monitor the entire delivery operation.

### Team Contributions

- **My Role:**
  - **Design and CAD Modeling:** Designed the robot's appearance and created a CAD model for 3D printing. The robot was printed in several parts, later assembled, and painted for a professional finish.  

  - **Autonomous Navigation Implementation:** Implemented the autonomous navigation system using a 2D LIDAR sensor and a Raspberry Pi camera for real-time video streaming. Integrated all subsystems using the ROS framework.

  ![ADBot: Autonomous Delivery Robot](https://manavthakkar.github.io/assets/images/adbot.jpeg)

- **Team Members:**
  - Collaborated on integrating hardware components and software systems.
  - Assisted in tuning navigation parameters and troubleshooting issues during testing.

### Technical Details

- **Technologies and Methodologies:**
  - **ROS (Robot Operating System):** Framework used for autonomous navigation and for connecting subsystems.
  - **2D LIDAR Sensor:** Primary sensor for navigation and obstacle avoidance.
  - **Raspberry Pi Camera:** For streaming real-time video feed.
  - **QR Code Authentication:** Secure delivery verification using unique QR codes.
  - **Servo Mechanism:** For unlocking the robot's door upon successful authentication.

### Challenges and Solutions

- **Tuning Navigation Parameters:** One of the main challenges was fine-tuning the autonomous navigation hyperparameters to ensure smooth operation within indoor environments. This required extensive trial and error but ultimately resulted in a well-functioning navigation system.
  
### Achievements and Recognition

- Our project was selected as the second-best in the Mechanical Engineering department at our university.
- Throughout the project, I shared our progress through a series of LinkedIn posts, covering various aspects from concept to autonomous navigation. Two of them were reposted by Open Robotics, the organization maintaining ROS, which greatly motivated me to pursue a career in robotics.

### Learning Outcomes

- Gained in-depth knowledge of ROS and autonomous navigation algorithms.
- Enhanced practical skills in designing, modeling, and assembling robotic components.
- Developed problem-solving skills through hands-on experience in tuning and optimizing navigation systems.

### LinkedIn Posts

1. [Concept](https://www.linkedin.com/posts/open-source-robotics-foundation_project-ros-technology-activity-6920412550727708672-o6te?utm_source=share&utm_medium=member_desktop)
2. [Manufacturing using 3D printing](https://www.linkedin.com/posts/manavt2000_3dprinting-robotics-amr-activity-6922137953884405760-YUPW/)
3. [Teleoperation](https://www.linkedin.com/posts/manavt2000_delivery-robot-amr-activity-6922869511616372736-_omh/)
4. [QR Code Authentication](https://www.linkedin.com/feed/update/urn:li:activity:6925658072698761216/)
5. [Map Building using Cartographer SLAM](https://www.linkedin.com/posts/open-source-robotics-foundation_slam-robotics-deliveryrobot-activity-6929844665529614336-7qFD?utm_source=share&utm_medium=member_desktop)
6. [Autonomous Navigation](https://www.linkedin.com/feed/update/urn:li:activity:6933326224974852096/)

These experiences and recognitions have significantly influenced my career path, solidifying my interest and commitment to the field of robotics.

