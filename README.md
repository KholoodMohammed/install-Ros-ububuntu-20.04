# install-Ros-ububuntu-20.04
Learn how to install Ros notice on Ubuntu 20.04 using Visual Box with steps
#Steps:
1. Download the visual box
2. Download Ubuntu20.04
Open visual box :
   *	Change settings
   *	Defining a new system to suit the device
   *	Choosing a Linux system to open Ubuntu20.04

3. Open and configure Ubuntu on the visual box
   *	Open the program on the device
   *	Fill in all the required data (account data - storage location - region - language ...)
4. Open Ubuntu and download Ros no into Ubuntu20.4
   Ros installation method:
   *	Open any browser inside Ubuntu20.04 and search for the steps to install Ros noetic  from the Ros  System website
   *	Open the terminal on Ubuntu.
   *	The Ros noetic install commands are copied command by order.
 #### Configure your Ubuntu repositories
   * Configure your Ubuntu repositories to allow "restricted," "universe," and "multiverse." You can follow the Ubuntu guide for instructions on doing this.
 #### Setup your sources.list
_Setup your computer to accept software from packages.ros.org._
 >  sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" >    /etc/apt/sources.list.d/ros-latest.list' 
   
 
 #### Set up your keys
 > sudo apt install curl # if you haven't already installed curl
 
 > curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
 #### Installation
 * First, make sure your Debian package index is up-to-date:
 >	sudo apt update
 *  Now pick how much of ROS you would like to install.
 *	Desktop-Full Install: (Recommended) : Everything in Desktop plus 2D/3D simulators and 2D/3D perception packages
 >	sudo apt install ros-noetic-desktop-full

 #### Environment setup
 
 * You must source this script in every bash terminal you use ROS in.
 
 > source /opt/ros/noetic/setup.bash
 
 **It can be convenient to automatically source this script every time a new shell is launched. These commands will do that for you.
     Bash**
     
 **f you have more than one ROS distribution installed, ~/.bashrc must only source the setup.bash for the version you are currently using .**
 
  > echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
  
  > source ~/.bashrc

  * Upon completion of the installation check by the word roscore
  > roscore
   
   


