# robotarm
## explanation of commands

This command is used to initialize the device to install ROS
```
$sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'  
```

To open the recv key in the device
```
$sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

Updated list, contains information about packages
```
$sudo apt-get update 
```
To install the full desktop version of the ROS for the Kinetic distribution
```
$sudo apt-get install ros-kinetic-desktop-full  
```

To searches for ROS packages available for installation on a Linux system
```
$apt-cache search ros-kinetic 
```

These two commands are run after installing ROS kinetic on Linux and are executed every time a new console window is opened to work on ROS kinetic
```
$echo "source /opt/ros/kinetic/setup.bash" >> ~/.bashrc
source ~/.bashrc
```

To install some necessary packages to run ROS programs on Linux
```
$sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential 
```

To install the python-rosdep package on Linux
```
$sudo apt install python-rosdep
```

To initialize ROS to use rosdep
```
$sudo rosdep init
```

To successfully update and run new packages on ROS
```
$rosdep update
```

This command installs the "ros-noetic-catkin" package on a Linux system
```
$sudo apt-get install ros-noetic-catkin
```

Create a new folder named “catkin_ws/src” using the mkdir command
```
$mkdir -p ~/catkin_ws/src
```

takes to the “~/catkin_ws/” directory using the cd command
```
$cd ~/catkin_ws/
```

Using this command to build my own work packages in Catkin workspace on ROS
```
$catkin_make
```

It takes me to the folder "~/catkin_ws/src" using cd command
```
$cd ~/catkin_ws/src
```

It leads to the package of the robot arm
```
$git clone https://github.com/smart-methods/arduino_robot_arm.git 
```

to switch to the working folder of the ROS package
```
$cd ~/catkin_ws
```

To run all packages that are required to run specific packages
```
$rosdep install --from-paths src --ignore-src -r -y
```

To install the moveit package in ROS kinetic using the system package manager apt-get
```
$sudo apt-get install ros-kinetic-moveit
```


`ros-kinetic-joint-state-publisher` used to publish the joint state of a given robot
`ros-kinetic-joint-state-publisher-gui` to visually display and control the state of the joints through the graphical interface
```
$sudo apt-get install ros-kinetic-joint-state-publisher ros-kinetic-joint-state-publisher-gui
```

`ros-kinetic-gazebo-ros-control` to control the Gazebo bot model with ROS Kinetic
`ros-kinetic-joint-state-publisher` to publish the joint state of a given robot
```
$sudo apt-get install ros-kinetic-gazebo-ros-control joint-state-publisher
```

`ros-kinetic-ros-controllers` to control the movement of robots in ROS
`ros-kinetic-ros-control` to create and run the observers
```
$sudo apt-get install ros-kinetic-ros-controllers ros-kinetic-ros-control
```

open the bashrc file, which is a file that runs internal programs at system startup
```
$sudo nano ~/.bashrc
```

This command is used to create the environment needed to run the ROS package
```
$(source /home/wafaa/catkin_ws/devel/setup.bash)
```

To reload the bashrc file
```
$source ~/.bashrc
```

This command is used to launch the ROS package and launch the robot_arm_pkg launch file “check_motors.launch”, which verifies that the motors of the robot arm are connected and operational
```
$roslaunch robot_arm_pkg check_motors.launch
```

## Run the simulator arm

![picture](robotarm.png)



























































ة’
ع
