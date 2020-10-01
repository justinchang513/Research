# Research
4_bar_walking_trajectory

Author: Justin Chang, Henry Chang, Nicholas Gravish
This is the research under Professor Nicholas Gravish's Bio-inspired Robotics. The current version is the code required to move the bipedal robots. The code right now is still under experimental phase; position vs current control. Position control is more absolute and gets the desired location in the most efficient way possible. However, this results in rigidity which could be problematic for obstacle-overcoming. With current control and virtual compliance, the body moves as if it's attached with virtual springs. Therefore, the mass has flexibility and has higher capability in obercoming obstacle.

The program is mainly split in three parts: odrive, kinematics, and main. 

Odrive: The main connection calibration and functions to communication with the Odrive motor driver. Moreover, the files for position, anisotropic, and isotropic walking gaits are included in the file. Lastly, the file plots the theoretical foot trajectories versus the realistic foot positions (as read from encoder readings). 

Kinematics: This highlights the leg geometry from the motors to the tip toe foot position. Included is also the current grid that allows the minimal current for both motors to sustain the toe's suspended position. Lastly, the file tracks the shape and speed of each foot trajectory.

Main: The main execution file. The main functions that are executed are the gait geometries with their respective control methods (positional, isotropic, and anisotropic).

This is the Jupyter version of the code as its easier to adjust and execute immediate control updates. Moreover, we are trying to switch to Arduino/C++ so microcontrollers with significantly better Baud rates and communication may be used. 
