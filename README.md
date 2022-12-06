# Turtlebot3-with-D435i-and-RplidarA1
This is a simple repository with Turtlebot3 with D435i urdf and RplidarA1

Please you get 
  
  >In Remote PCRealsense-ros https://github.com/IntelRealSense/realsense-ros
  
  >In Remote PCRplidar       https://github.com/Slamtec/rplidar_ros 

How to use it?
  
  >In Remote PC
  
   For Rplidar A1 : Replace package/turtlebot3_bringup/luanch
      $ roscd rplidar_ros/scripts/ &&  ./create_udev_rules.sh
      
      $ echo "export TURTLEBOT_LASER_SENSOR=rplidar" >> ~/.bashrc
      $ echo "source /home/ubuntu/catkin_ws/devel/setup.bash" >> ~/.bashrc
      
      $ ls -l /dev |grep ttyUSB
      $ sudo chmod 666 /dev/ttyUSB0
  
  >In SBC PC

    
-----------------------------------------------------------------------------------------------------------------------------      
  >In Remote PC
  
  >For D435i      : Replace package/turtlebot3_description/urdf/turtlebot3_waffle.urdf.xacro and join in the _d435.urdf.xacro and _d435.urdf.gazebo.xacro
 
