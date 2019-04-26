cmake_minimum_required(VERSION 2.8.3)
project(leo_system)

find_package(catkin REQUIRED COMPONENTS
  rospy
  std_msgs
)

catkin_package()

catkin_install_python(PROGRAMS 
   	 scripts/leo_system.py
	DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION})


