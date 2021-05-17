cmake_minimum_required(VERSION 2.8.3)

project(manipulator-kinematics)

find_package(catkin REQUIRED COMPONENTS roscpp rospy rviz tf2 tf2_ros geometry_msgs rosparam)

catkin_package()

include_directories(include ${catkin_INCLUDE_DIRS})

add_executable(manipulator-kinematics src/main.cpp)

target_link_libraries(manipulator-kinematics ${catkin_LIBRARIES})
