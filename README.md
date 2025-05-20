# Robot Arm Control with PID & Inverse Kinematics

## Project Overview

This project implements PID control and inverse kinematics for a robot arm in NVIDIA Isaac Sim. The implementation focuses on:

1. **PID Control** - Implementing PID controllers for accurate joint position control
2. **Inverse Kinematics** - Solving the inverse kinematics problem for trajectory planning

The code is designed to be developed locally and then run in Isaac Sim on an Azure Omniverse VM.

## Implementation Details

### Components

1. **PIDController** - A class that implements a PID controller for joint position control
2. **RobotArmKinematics** - Implements forward and inverse kinematics for a robot arm
3. **RobotArmController** - High-level controller combining PID and kinematics
4. **Main Program** - Demonstrates the robot arm following a square trajectory

#### Inverse Kinematics

Use Isaac Lab built in Differential IK controller class IKSolver.

## Running the Project

### Local Development

To run the simulation locally:

```bash
python main.py
```

This will run the simulation and output the robot arm's trajectory, position, and control signals.

### On Azure Omniverse VM

1. Clone the repository on your Azure VM


## Requirements

- Python 3.7+
- NumPy
- NVIDIA Isaac Sim (for the VM environment)

## Future Improvements

- Add collision avoidance
- Implement joint velocity and acceleration limits
- Add visualization tools
