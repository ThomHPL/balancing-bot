## Build
```
colcon build --symlink-install
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