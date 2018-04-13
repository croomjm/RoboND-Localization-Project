# RoboND-Localization-Project

This repository contains code for the Udacity Robotics Nanodegree localization project. To run, clone the git repository to the src folder in the [Udacity Ubuntu/ROS VM](https://s3-us-west-1.amazonaws.com/udacity-robotics/Virtual+Machines/Lubuntu_071917/RoboVM_V2.1.0.zip), make the directory, and source using Udacity VM devel/setup.bash.

The baseline robot configuration prescribed by Udacity can be run as follows:
`roslaunch udacity_bot udacity_world.launch`

My "upgraded" robot can be run as follows:
`roslaunch udacity_bot ultra_udacity_world.launch`

Both launch files have been modified to concurrently launch the [AMCL](http://wiki.ros.org/amcl#Subscribed_Topics) localization node as well.

In order to run the navigation_goal script, the following command should be run from catkin_ws in another terminal window:
`rosrun udacity_bot navigation`
