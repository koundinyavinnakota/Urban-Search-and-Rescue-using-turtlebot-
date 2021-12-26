# final_project
Non-complete package for the final project for: ENPM809Y Fall 2021

- The `doc` folder contains the instructions and the html documentation.
- The `script` folder contains install.bash to install required packages.

To run the package:
To set the ArUco markers:
- exportGAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/home/username/catkin_ws/src/final_project/models
-Place the package in you catkin workspace
- Build the package using catkin build final_project
Run the following commands to launch and simulate:
- roslaunch final_project multiple_robots.launch
- rosrun final_project final_project_node

