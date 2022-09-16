# The dumpbot_description package

- Author: Roberto Zegers
- License: BSD 3-Clause


## Description

This ROS2 package contains a mobile robot model of cuboidal base, differential drive kinematics and two caster wheels.

## Instructions

Clone this repo inside your ros2 workspace. Ensure you’re inside your workspace's `/src` directory before you clone.  
```
git clone https://github.com/rfzeg/dumpbot_description.git
```

Build and source the workspace.

```
colcon build --packages-select dumpbot_description
source install/setup.bash

```

To launch Rviz and display the robot model: 
```
ros2 launch dumpbot_description dumpbot_description.launch.py
```

To launch an empty Gazebo world and spawn the dumpbot robot:  
```
ros2 launch dumpbot_description gazebo.launch.py
```