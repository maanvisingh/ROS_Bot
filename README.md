# ROS Bot
The ROS bot is a differential drive outdoor bot that navigates autonomously. It uses ROS(Robot Operating System) to combine all the functionalities of the bot. 

## CAD
The Computer-Aided Design was created on SolidWorks Fusion 360.

## Manufacturing 
Parts of the base were first 3D printed individually and then assembled together. 

## Components 
- Microprocessor RasperrbyPi 4 Model B(Ubuntu 20.04 Server)
- Microcontroller Arduino UNO
- Lidar RPLidar A2
- IMU MPU 6050
- Mobile Power Bank
- Motor Driver L298N
- 2 Motors 
- 2 Motor Encoders 
- 2 Wheels 
- 2 Castor Wheels 

## Simulation
The CAD was first converted into a URDF(Unified Robotics Description Format) using [fusion2urdf](https://github.com/syuntoku14/fusion2urdf). This URDF model was then simulated in a gazebo world for initial testing. 

## Autonomous Navigation 
The laser scan data from the RPLidar is used for creating a map of the bot's environment based on Hector SLAM. 

## Codes
- ROS Package 
- Arduino Codes
