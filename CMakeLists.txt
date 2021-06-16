cmake_minimum_required(VERSION 2.8.3)
project(wally_launch)

find_package(catkin REQUIRED
        COMPONENTS roscpp ackermann_msgs nav_msgs)

find_package(Boost REQUIRED COMPONENTS random)

catkin_package(
  CATKIN_DEPENDS roscpp tf ackermann_msgs geometry_msgs nav_msgs
  DEPENDS system_lib
)

include_directories(${catkin_INCLUDE_DIRS})

