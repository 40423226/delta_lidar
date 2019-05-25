# How to build 3iRobotics Delta_2A Lidar ros package:
1) cd ~/catkin_ws/src/
2) git clone https://github.com/40423226/delta_lidar.git
3) cd ~/catkin_ws/
4) catkin_make
5) source ~/catkin_ws/devel/setup.bash
5) ls /dev/ttyUSB*
3) sudo chmod 666 /dev/ttyUSB0

# How to run 3iRobotics lidar rviz:
roslaunch  delta_lidar view_delta_lidar.launch

# How to run 3iRobotics lidar ros package:
* 2.1 ROS master:
```
roscore
```
* 2.1 run publish_node:
```
rosrun delta_lidar delta_lidar_node
```
or
```
roslaunch delta_lidar delta_lidar.launch
```
* 2.2 run subscribe_node:
```
rosrun delta_lidar delta_lidar_node_client
```