# All rights reserved.
cmake_minimum_required(VERSION 3.5)

### Export std_msgs/Headers
project(maritime_interfaces_support)

# Generate messages
find_package(ament_cmake_auto REQUIRED)
find_package(std_msgs REQUIRED)
find_package(sensor_msgs REQUIRED)

ament_auto_find_build_dependencies()

set(SUPPORT_INTERFACES
  shared/ComponentInfo.msg
  shared/FluidData.msg
)

rosidl_generate_interfaces(${PROJECT_NAME}
    ${SUPPORT_INTERFACES}

  DEPENDENCIES
    "std_msgs"
    "sensor_msgs"
  ADD_LINTER_TESTS
)

if(BUILD_TESTING)

endif()

ament_auto_package()

