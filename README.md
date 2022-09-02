Maritime Interfaces Standard
---
# Introduction
This outlines the standard for maritime interfaces

# Messages
## Engineering
| Component | Message                                                                                                  | Description                    |
| --------- | -------------------------------------------------------------------------------------------------------- | ------------------------------ |
| Engine    | [maritime_interfaces/msg/EngineConfig](/maritime_interfaces/engineering/engine/EngineConfig.msg)         | Configuration of an engine     |
| Engine    | [maritime_interfaces/msg/EngineState](/maritime_interfaces/engineering/engine/EngineState.msg)           | State of an engine             |
| Engine    | [maritime_interfaces/msg/EngineControl](/maritime_interfaces/engineering/engine/EngineControl.msg)       | Control of an engine           |
| Helm      | [maritime_interfaces/msg/HelmConfig](/maritime_interfaces/engineering/helm/HelmConfig.msg)               | Configuration of a helm        |
| Helm      | [maritime_interfaces/msg/HelmState](/maritime_interfaces/engineering/helm/HelmState.msg)                 | State of a helm                |
| Helm      | [maritime_interfaces/msg/HelmControl](/maritime_interfaces/engineering/helm/HelmControl.msg)             | Control of a helm              |
| Gearbox   | [maritime_interfaces/msg/GearboxControl](/maritime_interfaces/engineering/helm/GearboxControl.msg)       | Control of a gearbox           |
| Gearbox   | [maritime_interfaces/msg/GearboxState](/maritime_interfaces/engineering/helm/GearboxState.msg)           | State of a gearbox             |
| Gearbox   | [maritime_interfaces/msg/GearboxConstants](/maritime_interfaces/engineering/helm/GearboxConstants.msg)   | Constants for gearbox messages |
| Thruster  | [maritime_interfaces/msg/ThrusterControl](/maritime_interfaces/engineering/thruster/ThrusterControl.msg) | Thrust of an thruster          |
| Thruster  | [maritime_interfaces/msg/ThrusterState](/maritime_interfaces/engineering/thruster/ThrusterState.msg)     | Thrust of an thruster          |

## Sensors
### Common
| Sensor/s            | Message                                                                                                                                         | Description              |
| ------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------ |
| Battery             | [sensor_msgs/msg/BatteryState](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/BatteryState.msg)                           | Battery state            |
| IMU                 | [sensor_msgs/msg/Imu](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/Imu.msg)                                             | IMU data                 |
| Range Finder        | [sensor_msgs/msg/Range](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/Range.msg)                                         | Ranger data              |
| Satellite Fix (GPS) | [sensor_msgs/msg/NavSatFix](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/NavSatFix.msg)                                 | Sat Fix data             |
| Satellite Fix (GPS) | [sensor_msgs/msg/NavSatStatus](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/NavSatStatus.msg)                           | Sat Fix info             |
| Camera              | [sensor_msgs/msg/CameraInfo](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/CameraInfo.msg)                               | Camera info              |
| Camera              | [sensor_msgs/msg/Image](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/Image.msg)                                         | Camera data              |
| Camera              | [sensor_msgs/msg/CompressedImage](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/CompressedImage.msg)                     | Camera data (compressed) |
| AIS                 | [ais_msgs/msg/AisPositionReport](https://github.com/Greenroom-Robotics/ros_ais/blob/main/packages/ais_msgs/msg/AisPositionReport.msg)           |                          |
| AIS                 | [ais_msgs/msg/AisPositionReportRaw](https://github.com/Greenroom-Robotics/ros_ais/blob/main/packages/ais_msgs/msg/AisPositionReportRaw.msg)     |                          |
| AIS                 | [ais_msgs/msg/AisStaticDataReportRaw](https://github.com/Greenroom-Robotics/ros_ais/blob/main/packages/ais_msgs/msg/AisStaticDataReportRaw.msg) |                          |
| AIS                 | [ais_msgs/msg/AisVoyageRaw](https://github.com/Greenroom-Robotics/ros_ais/blob/main/packages/ais_msgs/msg/AisVoyageRaw.msg)                     |                          |
| Joystick            | [sensor_msgs/msg/Joy](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/Joy.msg)                                             |                          |
| Sonar               | [acoustic_msgs/msg/*](./maritime_interfaces/sensors/hydrographic_msgs/acoustic_msgs)                                                            |                          |

### Generic Support
| Message                                                                                                                                                 | Description    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| [sensor_msgs/msg/FluidPressure](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/FluidPressure.msg)                                 | Fluid Pressure |
| [sensor_msgs/msg/Temperature](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/Temperature.msg)                                     | Temperature    |
| [notification_msgs/msg/Notification](https://github.com/Greenroom-Robotics/ros_notifications/blob/main/packages/notification_msgs/msg/Notification.msg) |                |
| [maritime_interfaces/msg/ComponentInfo](maritime_interfaces/support/shared/ComponentInfo.msg)                                                           |                |
| [maritime_interfaces/msg/FluidData](maritime_interfaces/support/shared/FluidData.msg)                                                                   |                |


## Manouvre
| Message                                                                                                                                          | Description             |
| ------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------- |
| [sensor_msgs/msg/JointState](https://github.com/ros/common_msgs/blob/noetic-devel/sensor_msgs/msg/JointState.msg)                                | Orientation description |
| [geofence_msgs/msg/Geofences](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/Geofences.msg)             |                         |
| [geofence_msgs/msg/Geofence](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/Geofence.msg)               |                         |
| [geofence_msgs/msg/Polygon](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/Polygon.msg)                 |                         |
| [geofence_msgs/msg/UtmFences](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/UtmFences.msg)             |                         |
| [geofence_msgs/msg/UtmFence](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/UtmFence.msg)               |                         |
| [geofence_msgs/msg/UtmPolygon](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/UtmPolygon.msg)           |                         |
| [geofence_msgs/msg/UtmPolygon](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/geofence_msgs/msg/UtmPolygon.msg)           |                         |
| [geofence_msgs/srv/GeofencesUpdate](https://github.com/Greenroom-Robotics/ros_geofence/blob/main/packages/ros_geofence/srv/GeofencesUpdate.srv)  |                         |
| [waypoint_msgs/msg/Waypoint](https://github.com/Greenroom-Robotics/ros_waypoint/blob/main/packages/waypoint_msgs/msg/Waypoint.msg)               |                         |
| [waypoint_msgs/msg/Waypoints](https://github.com/Greenroom-Robotics/ros_waypoint/blob/main/packages/waypoint_msgs/msg/Waypoints.msg)             |                         |
| [waypoint_msgs/srv/WaypointsUpdate](https://github.com/Greenroom-Robotics/ros_waypoint/blob/main/packages/waypoint_msgs/srv/WaypointsUpdate.srv) |                         |


## Situational Awareness
| Message / Service                                                                                                                                                                           | Description                                              |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- |
| [perception_msgs/msg/BoundingBox2D ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/BoundingBox2D.msg)                                         | A 2D bounding box that can be rotated about its center.  |
| [perception_msgs/msg/ClassifiedRoi ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ClassifiedRoi.msg)                                         | A region of interest in an image with class information. |
| [perception_msgs/msg/ClassifiedRoiArray ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ClassifiedRoiArray.msg)                               | Message for a full set of classified ROIs                |
| [perception_msgs/msg/ImageChip ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ImageChip.msg)                                                 |                                                          |
| [perception_msgs/msg/ObjectClassification ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ObjectClassification.msg)                           |                                                          |
| [perception_msgs/msg/ObjectsFilter ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ObjectsFilter.msg)                                         |                                                          |
| [perception_msgs/msg/ObjectsPagination ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/ObjectsPagination.msg)                                 |                                                          |
| [perception_msgs/msg/Shape ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/Shape.msg)                                                         |                                                          |
| [perception_msgs/msg/TrackedObject ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/TrackedObject.msg)                                         |                                                          |
| [perception_msgs/msg/TrackedObjectKinematics ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/TrackedObjectKinematics.msg)                     |                                                          |
| [perception_msgs/msg/TrackedObjectWithChip ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/TrackedObjectWithChip.msg)                         |                                                          |
| [perception_msgs/msg/TrackedObjects ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/TrackedObjects.msg)                                       |                                                          |
| [perception_msgs/msg/TrackedObjectsWithChip ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/msg/TrackedObjectsWithChip.msg)                       |                                                          |
| [perception_msgs/srv/OBjectsHistory ](https://github.com/Greenroom-Robotics/ros_perception/blob/main/packages/perception_msgs/srv/OBjectsHistory.srv)                                       |                                                          |
| [geolocation_msgs/msg/Bound](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/msg/Bound.msg)                                                       |                                                          |
| [geolocation_msgs/msg/Location](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/msg/Location.msg)                                                 |                                                          |
| [geolocation_msgs/msg/RangeBearing](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/msg/RangeBearing.msg)                                         |                                                          |
| [geolocation_msgs/srv/GetCameraToCameraGrid](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetCameraToCameraGrid.srv)                       |                                                          |
| [geolocation_msgs/srv/GetGeobounds](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetGeobounds.srv)                                         |                                                          |
| [geolocation_msgs/srv/GetGroudSampleDistanceGrid](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetGroudSampleDistanceGrid.srv)             |                                                          |
| [geolocation_msgs/srv/GetHorizon](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetHorizon.srv)                                             |                                                          |
| [geolocation_msgs/srv/GetLocationFromPixel](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetLocationFromPixel.srv)                         |                                                          |
| [geolocation_msgs/srv/GetLocationFromPixelWithTopology](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetLocationFromPixelWithTopology.srv) |                                                          |
| [geolocation_msgs/srv/GetLocationFromRangeBearing](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetLocationFromRangeBearing.srv)           |                                                          |
| [geolocation_msgs/srv/GetPixelFromLocation](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetPixelFromLocation.srv)                         |                                                          |
| [geolocation_msgs/srv/GetPixelShiftsGrid](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetPixelShiftsGrid.srv)                             |                                                          |
| [geolocation_msgs/srv/GetRangeBearingFromPixel](https://github.com/Greenroom-Robotics/ros_geolocation/blob/main/packages/geolocation_msgs/srv/GetRangeBearingFromPixel.srv)                 |                                                          |

## Communications
| Message / Service                                                                                                                                                                                      | Description                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------- |
| [network_monitoring_interfaces/msg/BandwidthReportClient](https://github.com/Greenroom-Robotics/ros_network_monitoring/blob/main/packages/network_monitoring_interfaces/msg/BandwidthReportClient.msg) |                                                       |
| [network_monitoring_interfaces/msg/BandwidthReportServer](https://github.com/Greenroom-Robotics/ros_network_monitoring/blob/main/packages/network_monitoring_interfaces/msg/BandwidthReportServer.msg) |                                                       |
| [network_monitoring_interfaces/msg/NetworkStatistics](https://github.com/Greenroom-Robotics/ros_network_monitoring/blob/main/packages/network_monitoring_interfaces/msg/NetworkStatistics.msg)         |                                                       |
| [network_monitoring_interfaces/msg/PacketStatistics](https://github.com/Greenroom-Robotics/ros_network_monitoring/blob/main/packages/network_monitoring_interfaces/msg/PacketStatistics.msg)           |                                                       |
| [can_j1939_msgs/msg/*](https://github.com/Greenroom-Robotics/can_msgs/tree/main/packages/can_j1939_msgs/msg)                                                                                           | J1939 Standard Messages for GR Integration Service    |
| [nmea2000_msgs/msg/*](https://github.com/Greenroom-Robotics/can_msgs/tree/main/packages/nmea2000/msg)                                                                                                  | NMEA2000 Standard Messages for GR Integration Service |