# ROS_Installation_steps

Before installing ROS, we need to make a Virtual machine 

# Ubuntu_Installation

  1- Install Oracle Virtual Box 
  
  2- Create a new virtual machine and make the *type*  __Linux__ and the version  __Ubuntu__.

  3- Download Ubuntu 20.04.4 from link: https://releases.ubuntu.com/20.04/

  4- Right click on the Ubuntu Virtual machine you created then Settings then Storage then Controller IDE then Empty then click the disk icon on the right then     Choose a disk file, navigate to where the __Ubuntu 20.04.4 ISO__ file was downloaded and choose it. 


 Ubuntu has been sucessfully installed.  


# ROS_Installation_steps

1- Enter these commands in CMD:

             
      1- sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list' 
             
      2- sudo apt install curl
       
      3- curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
       
      4- sudo apt update
       
      5- sudo apt install ros-noetic-desktop-full
       
      6- source /opt/ros/noetic/setup.bash
      
      7- sudo apt install python3-rosdep python3-rosinstall python3-rosinstall-generator python3-wstool build-essential
      
      8- sudo apt install python3-rosdep
      
      9- sudo rosdep init
          rosdep update
             
             
 ROS has been sucessfully installed.   
 
 
 
 
 # FOR JETSON-NANO: 
 
  Jetson-Nano comes with Ubuntu installed. this guide will cover the installation of ROS1 on the Jetson-Nano. A link will be pasted at the end of this thread that will take you to an excellent guide by Q-Engineering that covers that very topic.



  ## ROS1 Installation Steps:

     Enter these commands in CMD:

      1- sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
      2- sudo apt install curl
      3- curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
      4- sudo apt update
      5- sudo apt install ros-melodic-desktop-full
      6- echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc
          source ~/.bashrc
      7- sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
      8- sudo apt install python-rosdep
      9- sudo rosdep init
          rosdep update

   ROS has been sucessfully installed on the Jetson-Nano. 
   
   Before using it, you need to have a workspace, to create a workspace.
   
   Check out this video made by Mahmoud Abdelgalil: https://www.youtube.com/watch?v=7QgjR6m-0KM (all credits to the owner of the video)
 
  Now ROS is ready to be used in projects.  
