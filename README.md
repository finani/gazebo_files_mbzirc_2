# gazebo_files_mbzirc_2
gazebo models, worlds and launch files for MBZIRC mission 2

1. copy 'mavros_posix_sitl.launch' file to ~/Firmware/Launch/

2. copy 'models' and 'worlds' folders to ~/Firmware/Tools/sitl_gazebo/

3. Add below to the ~/.bashrc



\# Set PX4 - Mavros - Gazebo\n
cd ~/catkin_ws/src/Firmware\n
source Tools/setup_gazebo.bash $(pwd) $(pwd)/build/px4_sitl_default\n
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$(pwd)\n
export ROS_PACKAGE_PATH=$ROS_PACKAGE_PATH:$(pwd)/Tools/sitl_gazebo\n
cd



※ simulation_mbzirc_release (world) is coded by HS Lee
