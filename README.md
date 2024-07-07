# 2-Wheeled Mobile Differential Drive Robot With ROS2 Humble


This project contains the necessary files to simulate a differential drive robot using ROS 2 and Gazebo. The robot model is defined using Xacro (XML Macros) and URDF (Unified Robot Description Format) files.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Usage](#usage)
- [Package Structure](#package-structure)
- [Dependencies](#dependencies)
- [Launch Instructions](#launch-instructions)
- [Contributing](#contributing)
- [License](#license)
- [Maintainers](#maintainers)

## Introduction
The `mobile_dd_robot` package simulates a differential drive robot in Gazebo. It uses ROS 2 for robot state publishing and control. This package includes the robot description files, Gazebo configuration, and necessary launch files.

## Installation

### Prerequisites
- ROS 2 Foxy Fitzroy or later
- Gazebo
- colcon build tool

### Steps
1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/mobile_dd_robot.git
    cd mobile_dd_robot
    ```

2. Install dependencies:
    ```bash
    rosdep install --from-paths src --ignore-src -r -y
    ```

3. Build the package:
    ```bash
    colcon build
    ```

4. Source the workspace:
    ```bash
    source install/setup.bash
    ```

## Usage
To launch the robot simulation in Gazebo:
```bash
ros2 launch mobile_dd_robot gazebo_model.launch.py
```

## Package Structure
- **launch/**: Contains launch files for starting the robot simulation in Gazebo.
- **model/**: Contains the robot description files (Xacro, URDF, and Gazebo configuration).
- **CMakeLists.txt**: The CMake build script.
- **package.xml**: Package metadata and dependencies.

## Dependencies
The `mobile_dd_robot` package depends on the following ROS 2 packages:
- `ament_cmake`
- `joint_state_publisher`
- `robot_state_publisher`
- `gazebo_ros`
- `xacro`
- `ros_gz_bridge`

These dependencies are specified in the `package.xml` file.

## Launch Instructions
1. Ensure all dependencies are installed and the package is built.
2. Source the workspace:
    ```bash
    source install/setup.bash
    ```
3. Launch the simulation:
    ```bash
    ros2 launch mobile_dd_robot gazebo_model.launch.py
    ```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch:
    ```bash
    git checkout -b feature-branch
    ```
3. Make your changes and commit them:
    ```bash
    git commit -m "Description of your changes"
    ```
4. Push to the branch:
    ```bash
    git push origin feature-branch
    ```
5. Create a pull request.

## License
This project is licensed under the [TODO: License declaration].

## Maintainers
- Syed Nazmus Sakib


