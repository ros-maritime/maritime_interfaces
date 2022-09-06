# All rights reserved.
cmake_minimum_required(VERSION 3.5)

### Export std_msgs/Headers
project(maritime_interfaces_engineering)

# Generate messages
find_package(ament_cmake_auto REQUIRED)
find_package(std_msgs REQUIRED)
find_package(maritime_interfaces_support REQUIRED)

ament_auto_find_build_dependencies()

set(ENGINE_INTERFACES
  engine/EngineConfig.msg
  engine/EngineControl.msg
  engine/EngineState.msg
)

set(GEARBOX_INTERFACES
  gearbox/GearboxConstants.msg
  gearbox/GearboxControl.msg
  gearbox/GearboxState.msg
)

set(HELM_INTERFACES
  helm/HelmControl.msg
  helm/HelmState.msg
)

set(THRUSTER_INTERFACES
  thruster/ThrusterControl.msg
  thruster/ThrusterState.msg
)

rosidl_generate_interfaces(${PROJECT_NAME}
    ${ENGINE_INTERFACES}
    ${GEARBOX_INTERFACES}
    ${HELM_INTERFACES}
    ${THRUSTER_INTERFACES}

  DEPENDENCIES
    "std_msgs"
    "maritime_interfaces_support"
  ADD_LINTER_TESTS
)

if(BUILD_TESTING)

endif()

ament_auto_package()

