cmake_minimum_required(VERSION 3.5)

project(maritime_interfaces_situational_awareness)

# Generate messages
find_package(ament_cmake_auto REQUIRED)
find_package(perception_msgs REQUIRED)
find_package(geolocation_msgs REQUIRED)

ament_auto_find_build_dependencies()

ament_auto_package()

