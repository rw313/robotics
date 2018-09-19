## Lab 1
**Rachel Wu (rww2115)**  
**David Lee (jl4397)**

*COMSW4733 Computational Aspects of Robotics*  
*Peter Allen*

#### To Run
This assumes that you have installed ROS Indigo on Ubuntu 14.04 and have cloned the [`rbx1` repository](https://github.com/pirobot/rbx1).

First, `cd` into this repository
```
$ cd lab1_rww2115_jl4397
```

Copy `timed_out_and_back.py` into your rbx1 repository. This will overwrite the `timed_out_and_back.py` that currently exists in rbx1.

```
$ cp timed_out_and_back.py <path to rbx1>/rbx1_nav/nodes/
```

*Note: if you don't want to overwrite the existing method: follow these instructions*
```
$ cd <path to rbx1>
$ git checkout -b lab1_rww2115_jl4397
$ cd <path to lab1_rww2115_jl4397>
$ cp timed_out_and_back.py <path to rbx1>/rbx1_nav/nodes/
```

To run the script, open three terminal windows. In one window, run
```
$ roslaunch rbx1_bringup fake_turtlebot.launch
```

In the second window, run
```
$ rosrun rviz rviz -d `rospack find rbx1_nav`/sim.rviz
```

In the final window, run
```
$ cd <path to rbx1>/rbx1_nav/nodes/
$ python timed_out_and_back.py
```

The program will prompt you for input. The letter T (lowercase or uppercase) will apply a translation on the robot in meters. The letter R (lowercase or uppercase) will apply a rotation on the robot in radians. The letter Q (lowercase or uppercase) will quit the program. CTRL-C will also quit the program.

#### Methods
Method: a brief descripon of your methods

#### Video
https://youtu.be/aAD4ArrrVSM
