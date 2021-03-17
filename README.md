# README for TURTLEBOT3 NAVIGATION PROJECT 

Author: Luxi Huang

## Project Overview:
This totally-from-scratch project involved modeling a Turtlebot3 in rviz and using Differential Drive Kinematics to perform Odometry calculations. 


The core project components are:

- rigid2d library containing 2D Lie Group operations for Transforms, Vectors and Twists as well as differential drive robot kinematics for odometry updates.
- nuturtle_description: houses the description of a differential drive robot with a caster wheel for support.
- nuturtle_robot: interfaces with the real Turtlebot3’s low-level controls such as setting wheel speeds and reading sensors.
- tsim: simulate turtle move by following certain waypoints.

## Dependencies
ROS Melodic 

##  HOW to install files:
### Option 1: 
1. Create a workspace 
  ``` 
    $ mkdir -p ~/catkin_ws/src 
    $ cd ~/catkin_ws/src
  ```

2. Download .rosinstall file to ```~catkin_ws\src``` directory
   
3. Use ```wstool``` to install all packages on ```.rosinstall``` file
  ```
  $ wstool update
  ```
   
4. catkin_make 
  ```
  $ catkin_make
  ```

  
### Option 2: 
1. create catkin_ws 
  
 ```
  $ mkdir -p ~/catkin_ws/src 
  $ cd ~/catkin_ws/src
```
2. clone all packages 
   
```
  $ git clone https://github.com/luxi-huang/Turtulebot3-Navigation.git
  $ git clone https://github.com/ME495-Navigation/nuturtlebot.git
```

3. catkin_make 
```
$ catkin_make
```

### How to run file:

[visit tsim package](https://github.com/luxi-huang/Sample_Code/tree/master/tsim) 