# SLAM with RTAB MAP

This project was done as part of assignments in Udacity Sofware Engineer Nanodegree. In this project, a 2D occupancy grid and 3D octomap are created from a simulated environment using a custom robot with the RTAB-Map package.RTAB-Map (Real-Time Appearance-Based Mapping) is a popular solution for SLAM to develop robots that can map environments in 3D. RTAB-Map has good speed and memory management, and it provides custom developed tools for information analysis. For this project we will be using the rtabmap_ros package, which is a ROS wrapper (API) for interacting with RTAB-Map.

### Prerequisites

This project has been written and tested in Ubuntu 16.04LTS using ROS Kinetic. 
RTAB-Map's ROS package needs to be installed before compiling the project. 

```
$ sudo apt-get install ros-kinetic-rtabmap-ros
```
ref: https://github.com/introlab/rtabmap_ros

### Installing

1- Clone the project and make sure to place the "map_my_world" and "teleop_twist_keyboard" folders in src folder of your catkin_ws

```
$ git clone https://github.com/andrewameri/ROS_Project_4_SLAM_WITH_RTABMAP.git
```
2- Go back to catkin_ws folder and make the project

```
$ cd ..
$ catkin_make
```

## Running the tests

1- Launch the nodes 
```
$ roslaunch map_my_world world.launch
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
$ roslaunch map_my_world mapping.launch
```
2- Navigate your robot in the simulation to create map for the environment! When you are all set, terminate the node and you could find your map db file in /root/.ros/ folder.

## Authors

* **Udacity** - *Initial code snippets * - [Udacity](https://www.udacity.com)
* **Andrew Ameri** - *Finalizing, building, and testing the project* - [andrewameri](https://github.com/andrewameri)



