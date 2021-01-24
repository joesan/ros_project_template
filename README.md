# ROS Project Template
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)
---
There is nothing interesting in this project, other than the fact that it is just a bare bones template for ROS based projects.

## Documentation

This README.md is organized using the DocToc npm plugin. Do the following steps to run the DocToc plugin against your set of README.md files:

- Install Node if you do not have it yet

- Install DocToc npm install -g doctoc

- CD into your project root folder and run doctoc .

## Pre-requisite

The project requires ROS Noetic and catkin, and is developed on Ubuntu 20.04 LTS.

- To install ROS please follow the tutorials from [here](http://wiki.ros.org/action/fullsearch/ROS/Tutorials): 

- To install catkin please follow the tutorials from [here](http://wiki.ros.org/catkin?distro=indigo#Installing_catkin)

- To install Gazebo to run the simulations, follow instructions from [here](http://gazebosim.org/tutorials?tut=install_ubuntu)

## How to build

Before building please ensure ROS Noetic and catkin are installed.  

```
mkdir -p ~/your_catkin_workspace/src
cd ~/your_catkin_workspace/
catkin_make
source devel/setup.bash
cd src/
```

You have to adapt to your catkin workspace name of your choice!

Afetr you cd into the src folder of this newly created workspace, checkout the source code for this project:

```
git clone https://github.com/joesan/ros_project_template.git
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
