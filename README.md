# Course Overview

In this course, you will learn the fundamentals of ROS2 through two engaging projects:
1. **Turtlesim Draw Shapes**: Learn to control a simulated turtle to draw various shapes.
2. **Autonomous SuperTuxKart**: Program a racing game to play autonomously using OpenCV.

Later, the course will be expanded to include **Autonomous SuperTuxKart with Imitation Learning**.

## Prerequisites

**Hardware:**
- A laptop running Windows 10/11 or Ubuntu 22.04 LTS.
- Minimum specifications: 8GB RAM, 30GB of available storage.

## Installation Instructions

*Note: If you are using Ubuntu 22, you can skip step 1.*

### Step 1: Install Ubuntu 22 for Windows (WSL)
1. Open PowerShell in Administrator mode.
2. Enter the following commands:

    wsl --install


    wsl --set-default-version 2

3. Reboot your computer.
4. Install Ubuntu 22 from the Microsoft Store, open it, and set a password (e.g., 123).

### Step 2: Update Ubuntu Packages
Open the Ubuntu terminal and run:

    sudo apt update && sudo apt upgrade -y

This command updates all the packages of the operating system.

### Step 3: Install Ansible
Ansible is a YAML-based automation tool that will install all necessary dependencies:

    sudo apt install -y ansible

### Step 4: Install Required Dependencies
Download the installation script using wget:

    wget https://fh-aachen.sciebo.de/s/hfe8Xv1X4wBPRo6/download -O install-webots_spot.yaml

Run the Ansible playbook to install dependencies:

    ansible-playbook install-webots_spot.yaml -e 'user=<your_username>' -e 'ansible_become_pass=<your_password>'

Replace <your_username> and <your_password> with your actual username and password.

## Course Content

*Each session will last 2-3 hours.*

1. **Introduction and Setup**  
   Learn the basics of Python programming, Linux terminal usage, and ROS2. We will also guide you through the installation of all required tools.
   - Hands-on session in: ros2_basics.ipynb

2. **Turtlesim with ROS2**  
   Explore the Turtlesim package in ROS2, and work on creating various shapes using provided hints.
   - Hands-on session in: ros2_turtlesim.ipynb

3. **Autonomous SuperTuxKart with ROS2 and OpenCV**  
   Use ROS2 and OpenCV to programmatically control SuperTuxKart. Compete with your peers for a fun and exciting learning experience.
   - Hands-on session in: ros2_stk.ipynb
