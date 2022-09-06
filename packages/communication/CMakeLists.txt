cmake_minimum_required(VERSION 3.5)

project(maritime_interfaces_communication)

# Generate messages
find_package(ament_cmake_auto REQUIRED)
find_package(network_monitoring_interfaces REQUIRED)

ament_auto_find_build_dependencies()

ament_auto_package()
