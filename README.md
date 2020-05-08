# Husky-Navigation-Stack-Custom
Customised the husky navigation stack with parameters and a custom map file.

To execute this:

sudo apt-get update
sudo apt-get install ros-kinetic-husky-desktop
sudo apt-get install ros-kinetic-husky-simulator

create a catkin workspace
put this package inside the src folder of the workspace
catkin_make or catkin build
source the workspace

Execute the following commands in different terminals :

  roslaunch husky_gazebo husky_empty_world.launch
  
  roslaunch mini_husky_2dnav move_base.launch
  
  roslaunch husky_viz view_robot.launch
  
  python nav_goals_to_husky.py
    Enter the x and y coordinates and the angle 
    
The robot moves automatically avoiding the obstacles (jackal_world map) and can plan a path on it's own.
  
  

