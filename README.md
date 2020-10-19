# ROS2Nav2
TurtleBot 3 ROS2 Navigation 2 Links & Scripts

# Links


# TurtleBot 3 ROS2 Foxy Navigation Sample App. ROS2 Foxy on Ubuntu Focal 20.04
Few modifications from available setup located @ https://navigation.ros.org/getting_started/index.html

Run script installFoxy2004TurtleBot3Nav2.sh to install ROS2 & Gazebo11 (TurtleBot3 is build from source in a workspace called dev_ws )

# Get script
cd ~

git clone https://github.com/chazyman/ROS2Nav2.git

# Make script executable
cd ~/ROS2Nav2

chmod +x installFoxy2004TurtleBot3Nav2.sh

# Will Install Foxy on Ubuntu Focal & install TurtleBot3 Source using latest Navigation Code
# Cherry pick entries from the script

# Run script
./installFoxy2004TurtleBot3Nav2.sh

# To run Sample in a Terminal run following commands
# Based on https://navigation.ros.org/getting_started/index.html 
# follow step 3 - 4 & Navigating see above link) 
# Make sure you position turtleBot3 in Rviz at a simalar location in the Gazebo World. 

# Look at the various multi terminal testing in file (Seperated by ----- or ----)
1 - Demo TurtleBot 3 Foxy With Nav2 and SLAMToolbox

# Dashing TutleBot3 for Dashing on Ubuntu 18.04
# TurtleBot 3 ROS2 Dashing Navigation Sample App. ROS2 Dashing on Ubuntu Bionic 18.04
Few modifications from available setup located @ https://navigation.ros.org/getting_started/index.html

Run script installDashing1804TurtleBot3Nav2.sh to install ROS2 & Gazebo9 (TurtleBot3 is build from source in a workspace called dev_ws )

# Get script
cd ~

git clone https://github.com/chazyman/ROS2Nav2.git

# Make script executable
cd ~/ROS2Nav2

chmod +x installDashing1804TurtleBot3Nav2.sh


# Run script
./installDashing1804TurtleBot3Nav2.sh

# To run Sample in a Terminal run following commands
#  
# follow step 3 - 4 & Navigating see above link) 
# Make sure you position turtleBot3 in Rviz at a simalar location in the Gazebo World. 


        source /usr/share/gazebo/setup.sh

        source ~/dev_ws/install/setup.bash

        export TURTLEBOT3_MODEL=waffle

        export GAZEBO_MODEL_PATH=$GAZEBO_MODEL_PATH:~/dev_ws/install/turtlebot3_gazebo/share/turtlebot3_gazebo/models

        ros2 launch nav2_bringup nav2_simulation_launch.py
