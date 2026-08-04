# Rosmaster-X3plus-development
Author: Vihaan Gangupanthulu

Used to store every task that is programmed for the Rosmaster X3plus robot

Rosmaster X3plus components:
  -Green anodized aluminum alloy body
  -6 DoF robotic arm
  -4ROS YDlidar
  -Raspberry Pi 5
  -Mecanum wheels
  -12V motors
  -Astra Pro Depth camera
  -ROS robot expansion board
  -7-inch screen
  -2 USB HUB expansion boards
  -LED strip

Beginning work:

To start with this robot, it was necessary first to assemble it using the different components that came out of the box. After completing mechanical assembly, there was also a necessity to learn about the robot and how to use all of the applications that came with the robot. This includes JupyterLab, MoveIT!, and RViz, which are all used to operate the robot's different sensors and cameras. JupyterLab is the main way to program different functions into the robot, and is what will be used to input all of the different tasks that will be made for the robot. MoveIT! is an application that allows for the simplification of using the robotic arm, allowing the creation of different functions that can control the arm's movement, which includes the position of the arm and the grippers. RViz is an application that lets me see the Lidar, and will allow for the detection of a 3d space around the robot.

Task #1: Complex Pick and Place

The first task for this robot is to integrate the different sensors and cameras that the robot has, including the Astra Proplus camera, 4ROS YdLidar, and the camera on the robotic arm, as well as the arm itself, to set a specific item anywhere in the room and utilize all the capabilities of the robot to go to the robot, pick it up, and set it in a specific area designated as base. 

Issue #1: The ~/run_docker command didn't work at all

Reason: Likely due to files for Docker being corrupted and permissions being disabled.

Solution: Rewrite the Raspberry PI 5 SD card so it is all new files.

Issue #2: When using run_docker, everything was set back to the presets, having X3 as the robot type, a1 as the LiDAR, and Astra_plus as the camera.

Reason: Resetting the SD card led to everything having the presets that were standard.

Solution: Use nano and the Bashrc file to change the presets back to what they were meant to be for the X3plus robot, having the robot type as X3plus, the LiDAR as 4ROS, and Astra_plus as the same because it was correct.

Issue #3: When trying to boot the Astra camera, it keeps on connecting and disconnecting.
Reason: Unknown
Solution: Unsolved


