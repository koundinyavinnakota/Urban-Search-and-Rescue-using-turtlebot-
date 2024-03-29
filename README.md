[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
# Search & Rescue using turtlebot

## Overview
This project is inspired by the the challenge of autonomous robotics for Urban Search and Rescue (US&R). In US&R after a disaster occurs, a robot is used to explore an unknown environment, such as a partially collapsed building, and locates trapped or unconscious human victims of the disaster (see examples of robots in below figure). The robot builds a map of the collapsed building as it ex- plores, and places markers in the map of where the victims are located. This map is then given to trained First Responders who use it to go into the building and rescue the victims.
  
US & R -  Robots             
:-------------------------:|
<img src="/resources/Search_recue_example.png" width="400" alt="Alt text" title=""> |

## Dependecies
- Ubuntu 20.04 LTS 
- ROS Noetic

## Installing catkin tools
```
sudo sh \
    -c 'echo "deb http://packages.ros.org/ros/ubuntu `lsb_release -sc` main" \
        > /etc/apt/sources.list.d/ros-latest.list'
wget http://packages.ros.org/ros.key -O - | sudo apt-key add -
sudo apt-get update
sudo apt-get install python3-catkin-tools

```
## Building the package
- Naviagate to you ros workspace and go into src
```
source /opt/ros/noetic/setup.bash
git clone https://github.com/koundinyavinnakota/Search-Rescue-using-turtlebot-.git
```
- To Install all dependencies 
```
cd final_project/script
sudo chmod a+rwx install.bash
./install.bash
cd ..
catkin build final_project
source /opt/ros/noetic/setup.bash
```
## To launch the simulation
-After building the project
- Naviagate to the workspace
```
source devel/setup.bash
roslaunch final_project multiple_robots.launch
```
- In a another terminal, navigate to ros1 workspace
```
source devel/setup.bash
rosrun final_project final_project_node
```

Gazebo & Rviz visual of the Simulation          
:-------------------------:|
<img src="/resources/Search_recue_example_1.png" width="400" alt="Alt text" title=""> |

#### Video of simulation [here](https://drive.google.com/file/d/1l2H_O-9uJx8seZBkI55smP-waWNU-k-K/view?usp=share_link)
