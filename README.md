[![Build Status](https://travis-ci.org/ros-drivers/velodyne.svg?branch=master)](https://travis-ci.org/ros-drivers/velodyne)

Overview
========

Velodyne<sup>1</sup> is a collection of ROS<sup>2</sup> packages supporting `Velodyne high
definition 3D LIDARs`<sup>3</sup>.

**Warning**:

  The master branch normally contains code being tested for the next
  ROS release.  It will not always work with every previous release.
  To check out the source for the most recent release, check out the
  tag `velodyne-<version>` with the highest version number.

The current ``master`` branch works with ROS Indigo and Kinetic.
CI builds are currently run for Lunar and Melodic but extensive
testing has not been completed in those environments.

- <sup>1</sup>ROS: http://www.ros.org
- <sup>2</sup>Velodyne: http://www.ros.org/wiki/velodyne
- <sup>3</sup>`Velodyne high definition 3D LIDARs`: http://www.velodynelidar.com/lidar/lidar.aspx

**安装方法**
```
  sudo apt-get install ros-kinetic-velodyne
  mkdir -p velodyneDriver/src && cd velodyneDriver/src
  git clone https://github.com/wangxizhe/velodyne.git
  cd ../..
  catkin_make
```
**运行方法**  
 ```
   source devel/setup.bash  
   64线
   roslaunch velodyne_pointcloud 64e_S3.launch  
   16线  
   roslaunch velodyne_pointcloud VLP16_points.launch  
