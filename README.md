# Face Tracker Application Using ROS & OpenCV
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
---

TODO: Documentation!

The idea is to combine the Raspi Motion Detection that I did a few years ago and ROS to control the navigation of a small Robot that can traverse my living room and the kitchen! I will expand on the Raspi Motiion Detection to identify objects and use that as a signal to help geo-locate my Robot and thus successfully navigate it. The goal is that it should move without any hindrance without any pre-knowledge of the environment.

Stay tuned for more!

## Pre-requisite

The project requires ROS Noetic and catkin, and is developed on Ubuntu 20.04 LTS.

- To install ROS please follow the tutorials from [here](http://wiki.ros.org/action/fullsearch/ROS/Tutorials): 

- To install catkin please follow the tutorials from [here](http://wiki.ros.org/catkin?distro=indigo#Installing_catkin)

- To install Gazebo to run the simulations, follow instructions from [here](http://gazebosim.org/tutorials?tut=install_ubuntu)

## How to build

Before building please ensure ROS Noetic and catkin are installed.  

```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
source devel/setup.bash
cd src/
```

Here I have named my workspace catkin_ws, but it could be anything of your choice!

Afetr you cd into the src folder of this newly created workspace, checkout the source code for this project:

```
git clone https://github.com/joesan/ros-face-tracker.git
cd ..
catkin_make
```

## Running Demo without launch file

To run the demo open a new terminal and type
```
roscore
```

To run talker open a new terminal and type
```
cd catkin_ws
source devel/setup.bash
rosrun beginner_tutorials talker
```

To run listener open a new terminal and type
```
cd catkin_ws
source devel/setup.bash
rosrun beginner_tutorials listener
```
To stop the program press ctrl+C in each of the three terminals.

## Running Demo using launch file

To run the demo using launch file type the following in a terminal

```
cd catkin_ws
source devel/setup.bash
roslaunch beginner_tutorials navo.launch
```

again utilize ctrl+C to stop program in each of the 2 terminal.
