# ROS Bot
The ROS bot is a differential drive outdoor bot that navigates autonomously. It uses ROS(Robot Operating System) to combine all the functionalities of the bot. The initial motivation behind this project is to have a hardware model on which ROS can be implemented and navigation algorithms be tested.

## CAD
The Computer-Aided Design was created on SolidWorks Fusion 360.


<img src="https://github.com/maanvisingh/RM_Taskphase/blob/main/Coding%20Tasks/Reference%20Image.png" width="400" >

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
The laser scan data from the RPLidar is used for creating a map of the bot's environment based on Hector SLAM. The odometry data from the onboard IMU and wheel encoder is used for localising the bot in the created map. Based on the combined data from the lidar, IMU and wheel encoders, the bot is given the appropriate velocity so as to navigate around obstacles.

## Codes
- ROS Package 
- Arduino Codes
