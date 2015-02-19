cmake_minimum_required(VERSION 2.8.3)
project(iai_urdf_msgs)

find_package(catkin REQUIRED COMPONENTS message_generation)

add_service_files(
  FILES
  AlterUrdf.srv
  SimpleAlterUrdf.srv
)

generate_messages(
  DEPENDENCIES
)


catkin_package(
  CATKIN_DEPENDS message_runtime
)