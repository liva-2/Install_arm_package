# Install_arm_package
# 1- Preparing ROS
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
# 2- Installing the package arduino_robot_arm
* Add the “arduino_robot_arm” package to “src” folder
```
 cd ~/catkin_ws/src
 sudo apt install git
 git clone https://github.com/smart-methods/arduino_robot_arm 
```
