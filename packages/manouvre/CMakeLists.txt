cmake_minimum_required(VERSION 3.5)

project(maritime_interfaces_manouvre)

# Generate messages
find_package(ament_cmake_auto REQUIRED)
find_package(geofence_msgs REQUIRED)
find_package(waypoint_msgs REQUIRED)
find_package(geolocation_msgs REQUIRED)

ament_auto_find_build_dependencies()

ament_auto_package()
