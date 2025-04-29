```
ros2 launch balancing_bot talker.launch.py
ros2 launch balancing_bot listener.launch.py
```


## Sending a static transform
Run command :
```
ros2 run tf2_ros static_transform_publisher 1 0.5 0.1 .8 0 0 world frame
```
Visualize in RViz2
``` 
ros2 run rviz2 rviz2
```
Add TF2, select world as fixed frame

## Broadcasting moving robot
Installing 
```
sudo apt install ros-jazzy-xacro ros-jazzy-joint-state-publisher-gui
```