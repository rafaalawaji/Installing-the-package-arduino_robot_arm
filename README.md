# installing the package arduino_robot_arm

in the first task we were asked to install ROS and the arduino robot arm package and control it 

1- sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'

2- sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654

3- sudo apt-get update

4- sudo apt-get install ros-melodic-desktop-full

5- apt-cache search ros-melodic

6- echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

7- source ~/.bashrc

8- sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential

9- sudo apt install python-rosdep

10- sudo rosdep init

11- rosdep update

12- sudo apt-get install ros-melodic-catkin

13- mkdir -p ~/catkin_ws/src

14- cd ~/catkin_ws/

15- catkin_make

16- cd ~/catkin_ws/src

17- git clone https://github.com/smart-methods/arduino_robot_arm.git 

18- cd ~/catkin_ws

19- rosdep install --from-paths src --ignore-src -r -y

20- sudo apt-get install ros-melodic-moveit

21- sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui

22- sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher

23- sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control

24- sudo nano ~/.bashrc

25- at the end of the (bashrc) file add the follwing line
(source /home/rafa/catkin_ws/devel/setup.bash)
then 
ctrl + o

26- source ~/.bashrc

27- roslaunch robot_arm_pkg check_motors.launch
