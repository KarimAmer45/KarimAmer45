# Hi, I'm Karim

I am a Mobile Robotics M.Sc. student focused on ROS2, Python, computer vision, planning, perception, teleoperation, and experimental robot systems.

My background combines robotics software with mechatronics, automation, electronics, and hands-on prototyping. I am especially interested in mobile robot autonomy, perception-driven systems, human supervision of robots, and field-ready experimental platforms.

## Portfolio Note

Some repositories here are older coursework, experiments, and local projects that I recently organized into a public robotics portfolio. I try to keep each README clear about what is implemented, what is simulated, and what still needs real-world validation.

## Current Focus

- ROS2-based robot interfaces and command pipelines
- Teleoperation, safety interfaces, and supervised autonomy
- Multi-robot coordination and experimental robot systems
- Planning, localization, mapping, and SLAM for mobile robots
- Computer vision for robot perception and pose estimation
- Practical integration of sensors, motors, embedded control, and robot software

## Selected Projects

> **Navigation:** the repos below are the ones worth clicking first. The `mobile-robotics-*` cluster are algorithm study implementations. Everything else is listed further down.

1. **[GNSS-Denied Visual-Inertial Localization](https://github.com/KarimAmer45/gnss-denied-visual-inertial-localization)**  
   EKF fusing IMU, visual odometry, and wheel odometry for localization during GNSS outages. Achieves 0.24 m position RMSE versus 26.65 m for dead-reckoning alone over a 34-second simulated outage. Includes Docker, regression tests, and an optional ROS 2 C++ wrapper.

2. **[ROS 2 C++ Teleoperation Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node)**  
   C++ `rclcpp` node with five independent safety guard layers: velocity clamp, acceleration limiter, deadman timeout, e-stop topic, and LaserScan obstacle stop. Safety callback benchmarked at 40 ns. Includes Gazebo Sim demo, CI, and 11 YAML-configurable parameters.

3. **[LLM-to-ROS 2 Command Interface](https://github.com/KarimAmer45/llm_to_ros)**  
   Tool-calling agent that translates natural language operator commands into validated, safety-clamped ROS 2 actions. Supports turtlesim and Gazebo backends, with schema validation, JSONL logging, and a mock motion planner.

4. **[Explainable Vision Demo](https://github.com/KarimAmer45/explainable-vision-demo)**  
   Transfer learning with ResNet, EfficientNet, and ViT-B/16, plus GradCAM and attention-rollout explainability overlays. Includes three Streamlit apps, CI, and a CIFAR-10 ViT experiment with reproducible metrics.

5. **[C++ Mobile Robot Kinematics](https://github.com/KarimAmer45/cpp-mobile-robot-kinematics)**  
   Dependency-free C++17 library for differential drive, mecanum, and Ackermann kinematics with SE(2) pose integration. Benchmarked at 74 M calls/sec for differential drive inverse kinematics.

6. **[Jetson-Ready ROS 2 Object Detection](https://github.com/KarimAmer45/jetson-ready-ros2-object-detection)**  
   ROS 2 Python detection node with Torchvision and YOLO backends, conditional Jetson/x86 Docker build arg, Ansible provisioning playbook, and DiagnosticStatus stats publishing.

7. **[Visual SLAM Evaluation — KITTI / EuRoC](https://github.com/KarimAmer45/visual-slam-evaluation-kitti-euroc)**  
   Evaluation toolkit for visual odometry and SLAM experiments: KITTI and EuRoC loaders, ORB VO baseline, Umeyama trajectory alignment, ATE/RMSE metrics, and trajectory plots. Docker included.

8. **[2D Occupancy Grid A* Visualizer](https://github.com/KarimAmer45/occupancy-grid-astar-visualizer)**  
   Dependency-free browser A* planner with interactive grid editor, npm unit tests, and an optional ROS 2 Gazebo Sim bridge that publishes `nav_msgs/OccupancyGrid` and `nav_msgs/Path`.

## More Projects

**ROS 2 & Systems**
- [ROS 2 Multi-Robot Coordination](https://github.com/KarimAmer45/ros2-multi-robot-coordination-demo) — coordinator/agent nodes, namespaced topics, waypoint assignment, Gazebo Sim
- [DJI ROS 2 Aerial Mapping Pipeline](https://github.com/KarimAmer45/dji-ros2-aerial-mapping-pipeline) — mission manifest intake, GeoJSON footprint export, ROS 2 handoff
- [Teleoperation Safety Interface](https://github.com/KarimAmer45/teleoperation-safety-interface) — browser HMI with safety interlocks, scenario presets, and GitHub Pages deployment
- [Robotics Edge Infra Lab](https://github.com/KarimAmer45/robotics-edge-infra-lab) — Ansible, Jetson provisioning, Jenkins CI, Docker for edge robotics nodes

**ML & Perception**
- [Machining Digital Twin Microservice](https://github.com/KarimAmer45/machining-digital-twin-microservice) — FastAPI service, Docker, live dashboard, Swagger UI
- [Machining Vibration ML](https://github.com/KarimAmer45/machining-vibration-ml) — physics-guided Random Forest for tool wear classification from vibration signals
- [Surface Roughness Signal Prediction](https://github.com/KarimAmer45/surface-roughness-signal-prediction) — RF regression on machining acoustic features, public dataset ready
- [UAV Building Footprint Extraction](https://github.com/KarimAmer45/uav-building-footprint-extraction) — k-means and MRF segmentation, polygon vectorization from aerial imagery

**Probabilistic Robotics**
- [FastSLAM](https://github.com/KarimAmer45/mobile-robotics-fastslam) · [EKF Localization](https://github.com/KarimAmer45/mobile-robotics-ekf-localization) · [Monte Carlo Localization](https://github.com/KarimAmer45/mobile-robotics-monte-carlo-localization) · [Occupancy Grid Mapping](https://github.com/KarimAmer45/mobile-robotics-occupancy-grid-mapping) · [Bayes Filter](https://github.com/KarimAmer45/mobile-robotics-bayes-filter) · [Odometry Motion Model](https://github.com/KarimAmer45/mobile-robotics-odometry-motion-model) · [Landmark Observation Model](https://github.com/KarimAmer45/mobile-robotics-landmark-observation-model)

**Planning & Classical CV**
- [C++ Grid Path Planner](https://github.com/KarimAmer45/cpp-grid-path-planner) · [MDP Value Iteration](https://github.com/KarimAmer45/mdp-value-iteration-planner) · [Grid Path Planning A*](https://github.com/KarimAmer45/grid-path-planning-astar)
- [Camera Calibration + Pose Demo](https://github.com/KarimAmer45/camera-calibration-pose-demo) · [Panorama Stitching](https://github.com/KarimAmer45/camera-calibration-panorama-stitching) · [Classical Image Processing](https://github.com/KarimAmer45/classical-image-processing-algorithms)
- [Graph Cut Segmentation](https://github.com/KarimAmer45/interactive-graph-cut-segmentation) · [Hough & Mean Shift](https://github.com/KarimAmer45/hough-mean-shift-segmentation) · [MOG People Tracking](https://github.com/KarimAmer45/mog-people-tracking) · [Kalman Filter Tracking](https://github.com/KarimAmer45/kalman-filter-tracking) · [Statistical Shape Modeling](https://github.com/KarimAmer45/statistical-shape-modeling)

## Technical Skills

**Robotics:** ROS2, mobile robotics, robot control, teleoperation, perception, planning  
**Programming:** Python, C++, MATLAB, JavaScript, Git, Linux  
**Computer Vision:** OpenCV, camera calibration, pose estimation, feature matching, segmentation  
**Algorithms:** A*, BFS, SLAM, FastSLAM, EKF, Monte Carlo localization, occupancy grids  
**Hardware and Automation:** sensors, motors, embedded control, Arduino, PCB design, PLC/SCADA  

## Research Interests

- Mobile robot autonomy
- Human-supervised robot operation
- Safety-aware teleoperation
- Multi-robot coordination
- Perception and planning for robot systems
- Field robotics and experimental platforms

## Contact

I am open to research assistant roles, thesis opportunities, and robotics projects involving ROS2, perception, planning, teleoperation, and experimental mobile robot systems.

[LinkedIn](https://www.linkedin.com/in/karim-amer-0546a2213/)  
Email: karimamer456@gmail.com
