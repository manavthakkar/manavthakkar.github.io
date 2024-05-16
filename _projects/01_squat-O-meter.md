---
name: Squat-O-Meter
tools: [Python, GUI, Signal Processing]
image: https://raw.githubusercontent.com/manavthakkar/squat-o-meter/main/screenshot.png
description: An app designed to help users track their squat exercises . It offers real-time feedback and voice notifications, making it a convenient tool for monitoring squat workouts.
---
# Squat-O-Meter: A Real-Time Squat Tracker GUI App

## Overview
Squat-O-Meter is a Python GUI application designed to help users track their squat exercises in real time using their mobile phone's accelerometer data. Developed using Tkinter and ttkbootstrap for the graphical user interface, this application provides a comprehensive solution for fitness enthusiasts to monitor their workout progress, set goals, and analyze their performance over time.

![Squat-O-Meter Screenshot](https://raw.githubusercontent.com/manavthakkar/squat-o-meter/main/screenshot.png)

## Key Features

1. **Real-Time Squat Detection:**
   - The user holds their mobile phone in their hands, extended in front, and the app uses accelerometer data to detect squats.
   - Data is transmitted over a local network using the Phyphox app.
   - Real-time squat count updates are displayed in the GUI.

2. **Feedback Mechanisms:**
   - Visual feedback is provided through the GUI, showing the updated squat count.
   - Voice feedback is available, with options to select different voices using the pyttsx3 library.

3. **Customizable Settings:**
   - Users can set a target number of squats before starting their workout.
   - Adjustable parameters include acceleration threshold and minimum time interval between squats to prevent false detections.
   - Users can choose to detect squats using either the z-direction acceleration or absolute acceleration, allowing flexibility in phone placement.

4. **Data Analysis and Progress Tracking:**
   - After completing a workout, users can save their squat count to a local database implemented using the pandas library.
   - The app includes a data analysis feature where users can view their progress over months, generate plots using matplotlib, and obtain various statistics such as total squats done, longest streak, and number of workout days.

   ![Analyze Data tab Screenshot](https://raw.githubusercontent.com/manavthakkar/squat-o-meter/main/Progress_Report.png)

## Technical Details

- **Libraries Used:**
  - **GUI:** Tkinter, ttkbootstrap
  - **Data Transmission:** Python requests module
  - **Data Plotting:** Matplotlib
  - **Signal Processing:** Scipy, Numpy
  - **Database Management:** Pandas, Datetime module
  - **Text-to-Speech:** Pyttsx3

- **Signal Processing:**
  - Incoming accelerometer data is processed to detect squats by identifying local minima based on user-set acceleration thresholds.
  - The app avoids false detections by enforcing a user-specified minimum time interval between squats.

- **User Interface:**
  - The GUI displays the real-time squat count and allows manual adjustment in case of false detections.
  - The "Analyze Data" tab enables users to plot and analyze their workout data, providing insights into their fitness progress.

## Challenges and Solutions
- **False Detection Handling:**
  - Implemented user-adjustable parameters for acceleration threshold and time interval between squats to minimize false positives.
  - Allowed manual adjustment of squat count in the GUI to correct any miscounts.

- **Data Transmission:**
  - Utilized the Phyphox app for reliable local network data transmission, ensuring smooth integration with the user's mobile phone.

## Future Improvements
- Adding support for additional exercises and extending the app’s capabilities to track different types of workouts.
- Incorporating more advanced data analysis features and machine learning algorithms to provide personalized workout recommendations.
- Enhancing the user interface with more customization options and interactive features.

This project showcases a robust and user-friendly application that leverages real-time data processing, customizable settings, and comprehensive data analysis to enhance the user's workout experience.


<p class="text-center">
{% include elements/button.html link="https://www.linkedin.com/feed/update/urn:li:activity:7187826427742879745/" text="Learn More" %}
</p>