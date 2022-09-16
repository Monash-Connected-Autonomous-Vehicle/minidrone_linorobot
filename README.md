# 🏎️ MiniDrone Simulator

This repository is a fork of the [linorobot2](https://github.com/linorobot/linorobot2) package for the purpose of simulating the [MCAV MiniDrone project](https://sites.google.com/student.monash.edu/minidrone).

## Installation

1. It is recommended to clone this repository into a separate ROS2 workspace. once you have created a workspace run `git clone https://github.com/Monash-Connected-Autonomous-Vehicle/minidrone_linorobot.git` from within the src folder.

2. Switch to the foxy branch with `git checkout foxy` from within the minidrone_linorobot folder

3. Install dependencies by running `rosdep update && rosdep install --from-path src --ignore-src -y --skip-keys microxrcedds_agent --skip-keys micro_ros_agent` from within the root of your workspace.

## How to run
1. After building the package and sourcing the workspace, run `ros2 launch linorobot2_gazebo minidrone.launch.py` to launch the simulator

2. To drive the robot, run `ros2 run teleop_twist_keyboard teleop_twist_keyboard` in a separate terminal

## Other
For more information on linorobot, see the LINOROBOT_README or view it on the linorobot2 repository