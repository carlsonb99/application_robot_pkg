# application_robot_pkg

This package includes a urdf (and xacro) file for a basic differntial robot, with two drive wheels and two fixed casters, as well as some launch files to view and operate the robot.

Dependancies include:  
*cpp_common  
rostime  
roscpp_traits  
roscpp_serialization  
catkin  
genmsg  
genpy  
message_runtime  
gencpp  
geneus  
gennodejs  
genlisp  
message_generation  
rosbuild  
rosconsole  
std_msgs  
rosgraph_msgs  
xmlrpcpp  
roscpp  
rosgraph  
rospack  
roslib  
rospy*  
  
Also used are:  
*urdf_tutorial  
xacro  
Gazebo*  
  
To bring up the robot in RViz, simply navigate to the application_robot_pkg and run:  
_roslaunch launch/display.launch_  

![Alt](/images/RViz_screen.png "RViz View")  

To bring up the robot in Gazebo, simply navigate to the application_robot_pkg and run:  
_roslaunch launch/gazebo.launch_  

![Alt](/images/gazebo_screen.png "Gazebo View")  

Here we can also pass arguments _m_ for angular velocity and _s_ for linear velocity. For example:  
_roslaunch launch/gazebo.launch m:=2.0 s:=1.0_  


![Alt](/images/gazebo_screen_circle.png "Gazebo Circle Driving View")  

This will make the robot drive in circles.  

