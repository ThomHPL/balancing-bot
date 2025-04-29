## Installation

:warning: This repo was made with ROS2 Jazzy and Gazebo Harmonic on an Ubuntu 24.04 Virtual Machine :warning:

### ROS2

Follow instructions from: https://docs.ros.org/en/jazzy/Installation/Ubuntu-Install-Debs.html

### Gazebo

```
sudo apt-get install ros-jazzy-ros-gz
```

## Build and source package
```
source /opt/ros/jazzy/setup.bash
colcon build --symlink-install

source install/setup.bash 
```

## Run in Gazebo
```
ros2 launch balancing_bot launch_sim.launch.py
```

## Run in Rviz
```
ros2 launch balancing_bot robot_state_publisher.launch.py
ros2 run rviz2 rviz2
ros2 run joint_state_publisher_gui joint_state_publisher_gui
```
Add TF and RobotModel manually, or use rviz file in `rviz/view_robot.rviz`

## TODO
- [ ] Differential wheels robot mode
    - [ ] look at gazebo bridge configuration
    - [ ] add keyboard control for simulation

- [ ] Balancing mode
    - [ ] add IMU sensor
    - [ ] add PID control