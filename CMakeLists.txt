cmake_minimum_required(VERSION 3.8)
project(curiosity_rover_description)
find_package(ament_cmake REQUIRED)

file(MAKE_DIRECTORY ${CMAKE_CURRENT_BINARY_DIR}/models/curiosity_path)

install(DIRECTORY
  models
  ${CMAKE_CURRENT_BINARY_DIR}/models
  DESTINATION share/${PROJECT_NAME}/
)

ament_package()
