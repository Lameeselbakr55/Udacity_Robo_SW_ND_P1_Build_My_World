# Udacity_Robo_SW_ND_P1_Build_My_World
A Simple World is Designed by Gazebo Ubuntu for Udacity Robotics Software Engineer Nanodegree Program 

The purpose of this project is to design a world with the Model Editor tool & Building Editor tool in Gazebo. Include this model in an empty Gazebo World. And, finally write a plugin to interact with this world.

### Directory Structure
The sample simulation world folder has the following directory structure:

    .Project1                                       # Build My World Project 
    ├── model                                    # Model files 
    │   ├── home
    │   │   ├── model.config
    │   │   ├── model.sdf
    │   ├── robot
    │   │   ├── model.config
    │   │   ├── model.sdf
    ├── script                                    # Gazebo World plugin C++ script      
    │   ├── Welcome.cpp
    ├── world                                   # Gazebo main World containing models 
    │   ├── Udacity_Office.world
    ├── CMakeLists.txt                     # Link libraries 
    └──                              


### Steps to launch the simulation


**Step 1 : Update and upgrade the Workspace image**	 

$ sudo apt-get update

$ sudo apt-get upgrade -y


**Step 2 : Clone the lab folder in /home/workspace/**

$ cd /home/workspace/

$ git clone https://github.com/Lameeselbakr55/Udacity_Robo_SW_ND_P1_Build_My_World.git

**Step 3 : Create a build directory and compile the code** 

$ cd ~/workspace/myrobot/

$ mkdir build

$ cd build/

$ cmake ../

$ make

**Step 4 : Add the library path to the Gazebo plugin path** 

$ export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:~/Project/build

(For my case: export GAZEBO_PLUGIN_PATH=${GAZEBO_PLUGIN_PATH}:/home/robond/workspace/Udacity_Robo_SW_ND_P1_Build_My_World/build)

**Step 5 : Run the Gazebo World file**

$ cd /home/robond/Desktop/workspace/RoboND-Build-My-World-P1/world

$ gazebo myworld

**Output**
 
![264965365_620108782636566_6606664975893924486_n](https://user-images.githubusercontent.com/98288035/150702474-7a2522b3-92ab-4ec4-81e6-dc41c0069cc4.jpg)

