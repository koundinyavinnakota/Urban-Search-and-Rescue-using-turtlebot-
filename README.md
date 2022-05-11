# Search & Rescue using turtlebot
In this project, showcases the simulation of search and rescue operation during disasters. There are two turtlebots, one as "explorer" and the other as "follower". The explorer job is to explore the area, build a map and locate victims (but in this project map is already built) and store the location of the victims, go back to startng point and pass the location date to the follower. The follower will then visit all locations which was passed by explorer and save/rescue the victims.

Steps to execute the project:

To run the package:
To set the ArUco markers:
- exportGAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:/home/username/catkin_ws/src/Search-Rescue-using-turtlebot--main/models
-Place the package in you catkin workspace
- Build the package using catkin build Search-Rescue-using-turtlebot--main

Run the following commands to launch and simulate:
- roslaunch final_project multiple_robots.launch
- rosrun final_project final_project_node

