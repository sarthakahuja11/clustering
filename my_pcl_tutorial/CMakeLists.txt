cmake_minimum_required(VERSION 2.8.3)
project(my_pcl_tutorial)

find_package(catkin REQUIRED COMPONENTS
  pcl_conversions
  pcl_ros
  roscpp
  sensor_msgs
)
include_directories(
  ${catkin_INCLUDE_DIRS}
)
add_executable(example src/example.cpp)
target_link_libraries(example ${catkin_LIBRARIES})
