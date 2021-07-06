# Install_arm_package
## 1- Preparing ROS
Create a workspace by using catkin_make
```
mkdir -p ~/catkin_ws/src
```
```
cd ~/catkin_ws/
```
```
catkin_make
```
```
echo "source ~/catkin_ws/devel/setup.bash" >> ~/.bashrc
```
```
source ~/.bashrc
```
## 2- Installing the package arduino_robot_arm
* Add the “arduino_robot_arm” package to “src” folder
```
 cd ~/catkin_ws/src
 ```
 ```
 sudo apt install git
 ```
 ```
 git clone https://github.com/smart-methods/arduino_robot_arm 
```
* nstall all the dependencies
```
cd ~/catkin_ws
```
```
rosdep install --from-paths src --ignore-src -r -y
```
```
sudo apt-get install ros-melodic-moveit
```
```
sudo apt-get install ros-melodic-joint-state-publisher ros-melodic-joint-state-publisher-gui
```
```
sudo apt-get install ros-melodic-gazebo-ros-control joint-state-publisher
```
```
sudo apt-get install ros-melodic-ros-controllers ros-melodic-ros-control
```
* Compile the package
```
catkin_make
```
## 3-Controlling the motors
```
roslaunch robot_arm_pkg check_motors.launch
```
## 4-now we able to controll the arm

