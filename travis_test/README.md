# PUT Motorsport Driverless recruitment task 2020

Task for new members of PUT Motorsport Driverless group. It consists three subtasks:
- building Canny edge detector 
- building image array to ROS Image message converter
- apply converter to camera and edge images and publish 

1. [Results of task](#results-of-task)
2. [Project requirements](#requirements)
3. [Workspace and project configuration](#configuration)

## Results of task
![results](./README_files/results.png)

## Requirements
- Ubuntu 18.04
- ROS Melodic
```bash
sudo apt install ros-melodic-desktop-full
```
- cv_bridge
```bash
sudo apt install ros-melodic-cv-bridge
```
- requirements.txt 
```bash
pip install -r requirements.txt 
```

## Configuration

### Make ROS workspace and get recruitment task repository
```bash
mkdir -p ~/dv_ws/src
cd ~/dv_ws/src
git clone https://github.com/PUT-Motorsport/PUTM_DV_recruitment_task_2020.git dv_task/
```

### Build workspace
```bash
cd ~/dv_ws
catkin_make
source devel/setup.bash
```

### Run node
```bash
roslaunch dv_task camera.launch
```
