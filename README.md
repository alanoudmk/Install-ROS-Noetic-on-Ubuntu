

# **Install ROS Noetic**


## **1. Ensure Your Windows 10 OS is Up to Date**
 > Settings -> System -> About
<img src="https://github.com/alanoudmk/Install-ROS-Noetic-on-WSL/assets/127528672/486e095d-68b7-4ca9-af96-f375bcaf0d60" width="200" height="100">

 It is recommended to update to Windows 10 or later for optimal performance.


***


## **2. Ensure you have downloaded Ubuntu**
We will be using Ubuntu version 20.04.6 for our work.
[How to Download Ubuntu](https://github.com/alanoudmk/Install-Ubuntu-20.04.6-On-VirtualBox) 


***



## **3.Install ROS Noetic 20.04**
- Installation command link for [ROS Noetic 20.04](https://wiki.ros.org/ROS/Installation).
- Select the [installation](https://wiki.ros.org/Installation) option.
- Select your platform. As we discussed, we will be using **Ubuntu 20.04.6**.
- <img src="https://github.com/alanoudmk/Install-ROS-Noetic-on-WSL/assets/127528672/f23c3c90-cbfe-433f-906b-702564c32876" width="200" height="80">


 Open the **Terminal** write the following commands: 
- Set up your Sources.list first.
    ```
   sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
   ```
- Set up your Keys
  ```
   sudo apt install curl # if you haven't already installed curl
   ```
   ```
   curl -s https://raw.githubusercontent.com/ros/rosdistro/master/ros.asc | sudo apt-key add -
   ```
- Installation _I personally recommend using the Desktop_Full installation_ .
   ```
  sudo apt update
   ```
  ```
  sudo apt install ros-noetic-desktop-full
  ```
- Enviroment Setup
  ```
  source /opt/ros/noetic/setup.bash
  ```
- To source ROS Noetic in every terminal and every session:
  ```
  source/opt/ros/noetic/setup.bash
  ```
  ```
  echo "source /opt/ros/noetic/setup.bash" >> ~/.bashrc
  ```
- To verify you downloaded correctly, write: 
   ```
   gedit ~/.bashrc
   ```
- Make sure you find _"source /opt/ros/noetic/setup.bash"_ at the end of the _.bashrc_file, as shown in the image below: 

<img src="https://github.com/alanoudmk/Install-ROS-Noetic-on-WSL/assets/127528672/5f56c79b-b2d6-47e7-a75e-bbe7ab86c023" width="400" height="40">
 

***



## **Useful Resources**

- [Full Instructions](https://wiki.ros.org/Installation/Ubuntu) provided by the ROS organization.
- YouTube playlist on ROS Noetic available [here](https://youtu.be/Qk4vLFhvfbI?si=vQ72YrGRS629p7wb).




 
