# ROS workspace with 2 UR3e robot simulation
A ROS workspace example with a simulation consisting in 2 UR3e robot sharing part of their workspace.
ROS version: Noetic
Targeted Ubuntu version: 20.04 LTS

# Installation
Clone this Git repository:
```
git clone <TO DO add the url>
```

Navigate to the cloned repository:
```
cd <TO DO add the path>
```

Install all the missing dependencies (if missing rosdep install it first):
```
rosdep install --from-paths src --ignore-src -r -y
```

Build the workspace:
```
catkin_make
```
or
```
catkin build
```

# Launching the simulation
Source the builded workspace:
```
source <path_to_workspace>/devel/setup.bash
```
Launch the simulation
```
roslaunch laboratorio_robotica_moveit_config_RG2 demo_gazebo.launch
```
Gazebo and RVIZ should pop up. You can plan and execute trajectories in RVIZ and check the execution in Gazebo.
