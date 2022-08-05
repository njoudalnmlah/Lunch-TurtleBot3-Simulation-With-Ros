# Setup 

### 1. Install Dependent ROS 1 Packages:
```
$ sudo apt-get install ros-noetic-joy ros-noetic-teleop-twist-joy \
ros-noetic-teleop-twist-keyboard ros-noetic-laser-proc \
ros-noetic-rgbd-launch ros-noetic-depthimage-to-laserscan \
ros-noetic-rosserial-arduino ros-noetic-rosserial-python \
ros-noetic-rosserial-server ros-noetic-rosserial-client \
ros-noetic-rosserial-msgs ros-noetic-amcl ros-noetic-map-server \
ros-noetic-move-base ros-noetic-urdf ros-noetic-xacro \
ros-noetic-compressed-image-transport ros-noetic-rqt* \
ros-noetic-gmapping ros-noetic-navigation ros-noetic-interactive-markers
```
### Install TurtleBot3 Packages :
```
$ sudo apt-get install ros-noetic-dynamixel-sdk
$ sudo apt-get install ros-noetic-turtlebot3-msgs
$ sudo apt-get install ros-noetic-turtlebot3
```

### 3. Set TurtleBot3 Model Name
```
$ echo "export TURTLEBOT3_MODEL=burger" >> ~/.bashrc
```
# Gazebo :
### 5. Install Gazebo Simulation Package :
```
$ cd ~/catkin_ws/src/
$ git clone -b noetic-devel https://github.com/ROBOTIS-GIT/turtlebot3_simulations.git
$ cd ~/catkin_ws && catkin_make
```
### 6. Launch Simulation World (burger)::

```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
```
### 7. Operate TurtleBot3:
```
$ roslaunch turtlebot3_teleop turtlebot3_teleop_key.launch
``` 
# SLAM
### install SLAM : 
``` 
$ sudo apt-get install ros-melodic-gmapping ros-melodic-navigation

``` 
###  on a new terminal that we already intiated,Lunch Simulation world  :
 
```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_gazebo turtlebot3_world.launch
 
```
### 10. Run SLAM node :
```
$ export TURTLEBOT3_MODEL=burger
$ roslaunch turtlebot3_slam turtlebot3_slam.launch slam_methods:=gmapping
 
```

#### 11. Run Teleoperation Node :
```
$ export TURTLEBOT3_MODEL=burger 
$ roslaunch turtlebot3_teleop turtlebot3_teleop turtlebot3_teleop_key.launch 
 
```


```
```
# Create And Save your Map 
#### 12. in a new terminal ,write the code below to save your map :
```
$ rosrun map_server map_saver -f -/map
 
 ```

![N](https://user-images.githubusercontent.com/107792107/183098438-7dd82942-8c06-4019-b0c2-b672418ef50c.jpg)



