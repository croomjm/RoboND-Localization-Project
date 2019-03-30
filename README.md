# RoboND-Localization-Project

I completed this project as part of [my Udacity Robotics Software Engineer Nanodegree](https://confirm.udacity.com/AQCTW57M). To complete the project, I deployed an adaptive particle filter (using the ROS AMCL library) to estimate a simulated roomba-like robot's position and orientation from wheel encoder signals and lidar sensor. I deployed code to simultaneously build a costmap from lidar data to map obstacles and used the ROS movebase package to generate feasible trajectories toward the goal position based on the costmap. My results are summarized in the [project report](./localization_project_report.pdf) (note: an academic-style paper rather than a detailed readme was required as part of the project).

This repository contains code for the Udacity Robotics Nanodegree localization project. To run, clone the git repository to the src folder in the [Udacity Ubuntu/ROS VM](https://s3-us-west-1.amazonaws.com/udacity-robotics/Virtual+Machines/Lubuntu_071917/RoboVM_V2.1.0.zip), make the directory, and source using Udacity VM devel/setup.bash.

The baseline robot configuration prescribed by Udacity can be run as follows:
`roslaunch udacity_bot udacity_world.launch`

My "upgraded" robot can be run as follows:
`roslaunch udacity_bot ultra_udacity_world.launch`

Both launch files have been modified to concurrently launch the [AMCL](http://wiki.ros.org/amcl#Subscribed_Topics) localization node as well.

In order to run the navigation_goal script, the following command should be run from catkin_ws in another terminal window:
`rosrun udacity_bot navigation_goal`

Videos of successful completion of the course can be found [here](https://youtu.be/rZfr-IhNei8) and [here](https://youtu.be/7aVs_MXItHM).
