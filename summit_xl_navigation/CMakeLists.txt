cmake_minimum_required(VERSION 3.5)
project(summit_xl_navigation)

find_package(ament_cmake REQUIRED)

install(
  DIRECTORY launch config params config_rviz
  DESTINATION share/${PROJECT_NAME}
)

ament_export_dependencies(${THIS_PACKAGE_INCLUDE_DEPENDS})
ament_package()
