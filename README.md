# 6wheeled-mobilerobot
6 wheeled mobile robot

cd catkin_ws
cd src
git clone https://github.com/rahulmsubramannian/6wheeled-mobilerobot.git
git clone https://github.com/ros-perception/slam_gmapping.git   *optional no need if gmapping already exists*
cd ..
catkin_make

copy catkin_ws/src/slam_gmapping/gmapping/launch/slam_gmapping_pr2.launch and paste in catkin_ws/src/mobile_robot_description/launch
change name to mapping.launch

source catkin_ws/devel/setup.bash
roslaunch mobile_robot_description gazebo.launch 

in new terminal

source catkin_ws/devel/setup.bash
roslaunch mobile_robot_description mapping.launch 

in new terminal

source catkin_ws/devel/setup.bash
rviz
