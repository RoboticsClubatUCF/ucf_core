# core_bringup
This package contains launch files to be used to bringup common nodes used in UCF workspaces.

#####Dependencies
<ul>
<li>usb_cam</li>
</ul>

## Table of Contents

[Launch Files](#launch)
  <ul>
  <li>[usb_cam.launch](#usb_cam)</li>
  </ul>

## <a name="launch"></a>Launch Files
Below is a brief description and use information for the various launch files contained in this package.

##### <a name="usb_cam" />usb_cam.launch

This launch file launches a <a href="http://wiki.ros.org/usb_cam" >usb_cam_node</a> to communicate with a usb camera ( specifically tested with c920 ). As of now the launch file must be passed a camera name(cam_name) and a camera port(cam_port). ROS needs write/read access to the cam_port. 

The launch file can be ran with following:

```
roslaunch core_bringup usb_cam.launch cam_name:=name_here cam_port:=/dev/videoX
```

To use the launch file within the vehicles minimal.launch add the following:

```
<include file="$(find core_bringup)/launch/usb_cam.launch>
  <arg name="cam_name" value="name_here" />
  <arg name="cam_port" value="/dev/videoX" />
</include>
```






