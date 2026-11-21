

# Pool Simulator

It is designed for underwater robots (ROV, AUV etc.). The model was created with olympic pool dimensions and includes a water volume with buoyancy.


## Requirements for use

- Ubuntu 24.04
- ROS 2 Jazzy
- Gazebo Harmonic (`gz-harmonic`)
- `ros-jazzy-ros-gz`

Install the Gazebo packages with:

```bash
sudo apt install ros-jazzy-ros-gz
```

## Installation

```bash
cd ~/ros2_ws/src
git clone <your-repo-url> pool_simulator
cd ~/ros2_ws
colcon build --packages-select pool_simulator
source install/setup.bash
```

## Launch Simulation in Gazebo
You can run the simulation with the following command.

```bash 
  ros2 launch pool_simulator gazebo.launch.xml
```

The simulation starts paused; press play in the Gazebo GUI to run it. The
launch file bridges `/clock` to ROS 2, so run your nodes with
`use_sim_time:=true`.
  
## Contact
- Tom Klappenecker - tom.klappenecker@gmail.com


## Credits and License
This package is adapted from
[cagdasaktay/pool-simulator](https://github.com/cagdasaktay/pool-simulator)
(MIT License, Copyright (c) 2021 cagdasaktay) and was ported from ROS Noetic
and Gazebo Classic to ROS 2 Jazzy and Gazebo Harmonic. It is released under
the MIT License; see [LICENSE](LICENSE).
  
