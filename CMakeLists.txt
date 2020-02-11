cmake_minimum_required(VERSION 2.8.3)
project(hero_msgs)

find_package(catkin REQUIRED COMPONENTS
  geometry_msgs
  message_generation
)

add_service_files(
  FILES
    GetBasePose.srv
)

catkin_package(
  CATKIN_DEPENDS message_runtime geometry_msgs
)

