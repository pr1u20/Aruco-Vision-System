# Aruco-Vision-System
This is a vision system to estimate the position of two robots in a playing table. It was developed for the Eurobot 2022, an international student robotics contest.

## Description
There is a camera connected to a Raspberry Pi with a view of the whole table: 
![map copy](https://user-images.githubusercontent.com/73555876/163551793-5a57cdea-362d-4e41-af64-7638e1adfb31.png)

There are Aruco tags on the samples and on top of the robots. The images captured are processed with Aru--.py file and the pose of the Aruco tags is calculated using OpenCV. An Euler Transformation is used to change the frame of reference from the camera's to the robots'. The position of the robot is sent using the nrf24l01+ transciever from the raspberri pi to the arduinos inside the robots.
