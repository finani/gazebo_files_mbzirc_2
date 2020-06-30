# gazebo_files_mbzirc_2
Firmware files(gazebo, launch) and darknet_ros files for MBZIRC mission 2

1. cp Firmware ~/catkin_ws/src/

2. cd darknet_ros/darknet_ros/yolo_network_config/weights && cat yolov3_mission2.tar.bz2.part* > yolov3_mission2.tar.bz2

3. tar -xvf yolov3_mission2.tar.bz2

4. cp darknet_ros ~/catkin_ws/src/darknet_ros
> Before you run the 4th command line, Go back to the root of the repository

#

\# Set PX4 - Mavros - Gazebo

```
# Set sitl_gazebo path
source ~/catkin_ws/src/Firmware/Tools/setup_gazebo.bash ~/catkin_ws/src/Firmware ~/catkin_ws/src/Firmware/build/px4_sitl_default
export ROS_PACKAGE_PATH=\$ROS_PACKAGE_PATH:~/catkin_ws/src/Firmware:~/catkin_ws/src/Firmware/Tools/sitl_gazebo
```
