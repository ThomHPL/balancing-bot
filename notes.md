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

creating custom robot with collision box and inertial matrices

## Simuating

Installing 

https://gazebosim.org/docs/all/ros2_gz_vendor_pkgs/
```
sudo apt-get install ros-jazzy-ros-gz
```

run state publisher with sim time:
```
ros2 launch my_bot rsp.launch.py use_sim_time:=true
```

test gazebo with
```
ros2 launch ros_gz_sim gz_sim.launch.py gz_args:=shapes.sdf
```

tuto from
https://automaticaddison.com/how-to-simulate-a-robotic-arm-in-gazebo-ros-2/#Joints

branch new gazebo of
https://github.com/joshnewans/articubot_one/tree/new_gazebo

migrating guide:
https://gazebosim.org/docs/latest/migrating_gazebo_classic_ros2_packages/