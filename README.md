# Multi-Agent Mapping

A ROS 2-based system for cooperative mapping and navigation using multiple TurtleBots.  
The goal is to scan the environment, detect obstacles (e.g., curbs), and build a shared map.

## Features
- ROS 2 dataset reader (stream and time-range modes)
- Multi-sensor data synchronization (Lidar, IMU, Camera, etc.)
- Architecture prepared for multi-agent task allocation
- Extensible for SLAM integration and route optimization

## 📁 Project Structure

The project is organized into modular components to support simulation, SLAM, multi-agent coordination, and planning.

multi-agent-mapping/
├── src/
│   ├── ros2_data_reader/      # ROS 2 bag reader and sensor data parsing
│   ├── mapping/               # SLAM algorithms, map merging, and processing
│   ├── multi_agent_nav/       # Multi-agent coordination and task allocation
│   ├── planning/              # Path planning and goal assignment
│   ├── simulation/            # Simulation setup for multiple TurtleBots
├── config/                    # Configuration files (topics, parameters, robot models)
├── launch/                    # ROS 2 launch files for system components
├── data/                      # Bag files, generated maps, logs
├── notebooks/                 # Jupyter notebooks for debugging, visualization, and analysis
├── README.md                  # Project documentation
├── LICENSE                    # MIT License
└── requirements.txt           # Python dependencies

