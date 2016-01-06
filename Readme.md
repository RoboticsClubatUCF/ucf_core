# ucf_core
Workspace containing anything platform independent for UCF Robotics Club vehicles.  Primarily sensors such as cameras and lasers that may be common to every platform.

## Table of Contents
[Packages](#packages)

## <a name="packages"></a>Packages
Below is a brief description of and links to the various ROS packages in this workspace.
* [core_description](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core/core_description) -- URDF descriptions for components common between vehicles like sensors.
* [waypoint_manager](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_apps/waypoint_manager) -- Simple waypoint tracking package supporting navigation in order to a set of waypoints.
* [waypoint_manager_msgs](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_apps/waypoint_manager_msgs) -- Messages, services, etc used by the [waypoint_manager](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_apps/waypoint_manager) package.
* [core_cameras](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/core_cameras) -- Support including drivers and launch files for cameras used on club vehicles.
* [core_gps](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/core_gps) -- Extra layer of abstraction for use of community developed GPS support.
* [core_hokuyo](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/core_hokuyo) -- Extra layer of abstraction for use of the [hokuyo_node](http://wiki.ros.org/hokuyo_node) package on club vehicles.
* [core_sparton](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/core_sparton) -- Drivers and support for Sparton IMU/GPS devices.
* [roboteq_driver](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/roboteq_driver) -- Club modification of the [roboteq_driver](http://wiki.ros.org/roboteq_driver) package.
* [roboteq_msgs](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/roboteq_msgs) -- Message support for the [roboteq_driver](https://github.com/RoboticsClubatUCF/ucf_core/tree/master/src/core_drivers/roboteq_driver) package.
