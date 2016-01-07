# ucf_core
Workspace containing anything platform independent for UCF Robotics Club vehicles.  Primarily sensors such as cameras and lasers that may be common to every platform.

## Table of Contents
* [Packages](#packages)
* [Getting Started](#getting-started)

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

## <a name="getting-started"></a>Getting Started
If you're completely new, follow these steps to get up and running with our current builds.

1. Set up your development environment.  You need to be running Ubuntu 14.04 and have ROS installed.  Ubuntu installs end up being fairly unique, so we leave that to [google](http://google.com).  To get ROS set up propertly, see Chapter 2 of [this book available freely online](http://www.cse.sc.edu/~jokane/agitr/).  We have no official IDE supported by club members currently, but QtCreator and Eclipse both seem to work ok if you search around for configurations.  Your text editor of choice is the easiest option.

2. Become familiar with basic ROS functionality including how to build existing packages and create new ones.  The book linked above is an excellent resource for getting started and a fairly short read.

3. Fork (recommended if you're looking to get involved in development) and clone this repository.

4. Build ucf_core first.
  1. In a terminal navigate to ../ucf_robotics/ucf_core/ , enter the following:
    
    `rosdep install -i -y --from-paths src`
    
  2. Now `catkin_make` and `source devel/setup.bash` like usual.
  
5. In the same terminal window where you have sourced the ucf_core setup.bash, navigate to any other workspaces you want to build ( ie. ucf_igvc, ucf_boat, ucf_sub ).

6. Perform the same `rosdep install` as shown in step 4, build, and source to use.
