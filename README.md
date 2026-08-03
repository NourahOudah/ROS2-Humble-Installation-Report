# ROS2-Humble-Installation-Report
A step-by-step installation report for Ubuntu 22.04 LTS and ROS 2 Humble using WSL.
# ROS 2 Humble Installation Report

## Student Information

- Course: Robotics
- Assignment: ROS 2 Installation Report

---

# Introduction

This report explains the installation process of Ubuntu 22.04 LTS and ROS 2 Humble using Windows Subsystem for Linux (WSL). The installation was completed successfully by following the provided instructions.

---

# Step 1: Install Ubuntu 22.04

The installation started by enabling Windows Subsystem for Linux (WSL) and downloading Ubuntu 22.04 LTS.

<img src="./images/pcer1.png" width="600">

---

# Step 2: Create a Linux User

After the installation finished, a new Linux username and password were created.

![Step 2](images/pcter2.png)

---

# Step 3: Verify Ubuntu Version

The Ubuntu version was verified using the following command:
lsb_release -a

The result confirmed that the installed version is Ubuntu 22.04 LTS.

![Step 3](images/pcter3.png)

---

# Step 4: Update Ubuntu

The operating system packages were updated before installing ROS 2.
sudo apt update && sudo apt upgrade

![Step 4](images/pc4.png)

---

# Step 5: Install Required Packages

The required packages were installed before installing ROS 2.
sudo apt install software-properties-common curl

![Step 5](images/pc5.png)

---

# Step 6: Install ROS 2 Humble

ROS 2 Humble Desktop was installed successfully.
sudo apt install ros-humble-desktop

![Step 6](images/pc5.png)

---

# Step 7: Configure ROS 2

ROS 2 was added to the bash configuration file.
echo "source /opt/ros/humble/setup.bash" >> ~/.bashrc
source ~/.bashrc

![Step 7](images/pcer12.png)

---

# Step 8: Verify ROS 2 Installation

The installation was verified using:
echo $ROS_DISTRO

The output was:
humble

This confirms that ROS 2 Humble was installed successfully.

![Step 8](images/pcter11.png)

---

# Problems Encountered

During the installation, the following issues were encountered:

- A package name was typed incorrectly (`software-properties-common`), which caused an installation error.
- The issue was resolved by correcting the package name and running the command again.
- The command ros2 --version did not display the ROS version, so the installation was verified using:
echo $ROS_DISTRO

The output was:
humble

---

# Conclusion

Ubuntu 22.04 LTS and ROS 2 Humble were installed successfully. All required installation steps were completed, and the final verification confirmed that the ROS distribution is Humble.
