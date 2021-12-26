----> Steps to execute the project

To run the package:
To set the ArUco markers:
- exportGAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/home/username/catkin_ws/src/final_project/models
-Place the package in you catkin workspace
- Build the package using catkin build final_project

Run the following commands to launch and simulate:
- roslaunch final_project multiple_robots.launch
- rosrun final_project final_project_node

