<div align="center">

# Karim Amer

**Mobile Robotics M.Sc. · ROS 2 · C++ · Python · Computer Vision**

Building production-quality robot software: sensor fusion, safety systems, LLM-to-robot interfaces, and ML perception pipelines.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karim-amer-0546a2213/)
[![Email](https://img.shields.io/badge/Email-karimamer456%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:karimamer456@gmail.com)

![ROS2](https://img.shields.io/badge/ROS_2-22314E?style=flat-square&logo=ros&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B17-00599C?style=flat-square&logo=c%2B%2B&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

<br/>

[![GitHub stats](https://github-readme-stats.vercel.app/api?username=KarimAmer45&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github)](https://github.com/KarimAmer45)
[![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=KarimAmer45&layout=compact&theme=tokyonight&hide_border=true&langs_count=6)](https://github.com/KarimAmer45)

</div>

---

## Benchmarks at a Glance

All numbers are reproducible — each repo README has the exact command.

| Project | What was measured | Result |
|---|---|:---:|
| [GNSS-Denied VIO](https://github.com/KarimAmer45/gnss-denied-visual-inertial-localization) | EKF position RMSE vs. dead-reckoning over a 34 s outage | **0.24 m** vs. 26.65 m · 99.1% better |
| [ROS 2 Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node) | C++ safety-filter callback · 10 M iterations · `-O2` | **40 ns · 24 M calls/sec** |
| [C++ Kinematics](https://github.com/KarimAmer45/cpp-mobile-robot-kinematics) | Differential drive inverse kinematics throughput | **74 M calls/sec · 13.6 ns/call** |
| [C++ Grid Planner](https://github.com/KarimAmer45/cpp-grid-path-planner) | A\* vs. Dijkstra on a 500 × 500 grid | **11.3× faster · 15.6 ms vs. 176 ms** |
| [Explainable Vision](https://github.com/KarimAmer45/explainable-vision-demo) | ViT-B/16 fine-tuned on CIFAR-10 airplane vs. ship | **98% accuracy · AUC 0.994 · mAP 0.993** |
| [Pose Estimation](https://github.com/KarimAmer45/camera-calibration-pose-demo) | solvePnP on 30 synthetic chessboard frames | **214 FPS · 4.0 ms median** |

---

## Visual Results

<table>
<tr>
<td align="center" width="50%">

**[GNSS-Denied Visual-Inertial Localization](https://github.com/KarimAmer45/gnss-denied-visual-inertial-localization)**

EKF fusing IMU, visual odometry, and wheel odometry keeps the trajectory tight while dead-reckoning drifts 26 m during a 34-second satellite blackout.

![Trajectory overview](https://raw.githubusercontent.com/KarimAmer45/gnss-denied-visual-inertial-localization/main/results/example/trajectory_overview.png)

</td>
<td align="center" width="50%">

**[ROS 2 C++ Teleoperation Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node)**

Five independent C++ guard layers — velocity clamp, acceleration limit, deadman timeout, e-stop, and obstacle stop — running live in Gazebo Sim.

![Safety node demo](https://raw.githubusercontent.com/KarimAmer45/ros2-cpp-teleop-safety-node/main/docs/demo.gif)

</td>
</tr>
<tr>
<td align="center" width="50%">

**[LLM → ROS 2 Command Interface](https://github.com/KarimAmer45/llm_to_ros)**

Tool-calling agent translates natural language operator intent into schema-validated, safety-clamped ROS 2 actions across turtlesim and Gazebo backends.

![LLM to ROS demo](https://raw.githubusercontent.com/KarimAmer45/llm_to_ros/main/docs/demo.gif)

</td>
<td align="center" width="50%">

**[Explainable Vision Demo](https://github.com/KarimAmer45/explainable-vision-demo)**

ResNet, EfficientNet, and ViT-B/16 training with GradCAM and attention-rollout overlays. Streamlit UI for interactive inference and explainability inspection.

![GradCAM example](https://raw.githubusercontent.com/KarimAmer45/explainable-vision-demo/main/docs/screenshots/gradcam_example.png)

</td>
</tr>
<tr>
<td align="center" width="50%">

**[UAV Building Footprint Extraction](https://github.com/KarimAmer45/uav-building-footprint-extraction)**

K-means coarse mask followed by MRF energy minimisation and polygon vectorisation from UAV aerial imagery.

![UAV footprint overlay](https://raw.githubusercontent.com/KarimAmer45/uav-building-footprint-extraction/main/data/img_mosaic_overlay_polys.png)

</td>
<td align="center" width="50%">

**[ROS 2 Multi-Robot Coordination](https://github.com/KarimAmer45/ros2-multi-robot-coordination-demo)**

Coordinator and agent nodes with namespaced topics, dynamic waypoint assignment, and Gazebo Sim integration.

![Multi-robot demo](https://raw.githubusercontent.com/KarimAmer45/ros2-multi-robot-coordination-demo/main/docs/demo.gif)

</td>
</tr>
</table>

---

## Selected Projects

> **Navigation:** the repos below are the ones worth clicking first. The `mobile-robotics-*` cluster are algorithm study implementations — listed further down under Probabilistic Robotics.

| | Project | Highlights |
|---|---|---|
| 🔵 | **[GNSS-Denied Visual-Inertial Localization](https://github.com/KarimAmer45/gnss-denied-visual-inertial-localization)** | EKF sensor fusion · Docker · ROS 2 C++ wrapper · regression tests · 0.24 m outage RMSE |
| 🔵 | **[ROS 2 C++ Teleoperation Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node)** | 5 guard layers · 40 ns callback · CMake · CI · Gazebo Sim · 11 YAML params |
| 🔵 | **[LLM → ROS 2 Command Interface](https://github.com/KarimAmer45/llm_to_ros)** | Tool-calling · safety clamp · schema validation · JSONL logging · turtlesim + Gazebo |
| 🔵 | **[Explainable Vision Demo](https://github.com/KarimAmer45/explainable-vision-demo)** | ResNet · EfficientNet · ViT · GradCAM · attention rollout · 3 Streamlit apps · CI |
| 🔵 | **[C++ Mobile Robot Kinematics](https://github.com/KarimAmer45/cpp-mobile-robot-kinematics)** | Diff drive · mecanum · Ackermann · SE(2) · 74 M calls/sec · header-only C++17 |
| 🔵 | **[Jetson-Ready ROS 2 Object Detection](https://github.com/KarimAmer45/jetson-ready-ros2-object-detection)** | Torchvision + YOLO · Dockerfile · Ansible · DiagnosticStatus · Jetson build arg |
| 🔵 | **[Visual SLAM Evaluation — KITTI / EuRoC](https://github.com/KarimAmer45/visual-slam-evaluation-kitti-euroc)** | KITTI + EuRoC loaders · ORB VO · Umeyama alignment · ATE/RMSE · Docker |
| 🔵 | **[2D Occupancy Grid A\* Visualizer](https://github.com/KarimAmer45/occupancy-grid-astar-visualizer)** | Vanilla JS · npm tests · interactive editor · optional ROS 2 Gazebo Sim bridge |

---

## More Projects

**ROS 2 & Systems**
- [ROS 2 Multi-Robot Coordination](https://github.com/KarimAmer45/ros2-multi-robot-coordination-demo) — coordinator/agent nodes, namespaced topics, waypoint assignment, Gazebo Sim
- [DJI ROS 2 Aerial Mapping Pipeline](https://github.com/KarimAmer45/dji-ros2-aerial-mapping-pipeline) — mission manifest intake, GeoJSON footprint export, ROS 2 handoff
- [Teleoperation Safety Interface](https://github.com/KarimAmer45/teleoperation-safety-interface) — browser HMI, safety interlocks, scenario presets, GitHub Pages
- [Robotics Edge Infra Lab](https://github.com/KarimAmer45/robotics-edge-infra-lab) — Ansible, Jetson provisioning, Jenkins CI, Docker for edge nodes

**ML & Perception**
- [Machining Digital Twin Microservice](https://github.com/KarimAmer45/machining-digital-twin-microservice) — FastAPI, Docker, live dashboard, Swagger UI
- [Machining Vibration ML](https://github.com/KarimAmer45/machining-vibration-ml) — physics-guided Random Forest for tool wear classification from vibration signals
- [Surface Roughness Signal Prediction](https://github.com/KarimAmer45/surface-roughness-signal-prediction) — RF regression on machining acoustic features, public dataset ready
- [UAV Building Footprint Extraction](https://github.com/KarimAmer45/uav-building-footprint-extraction) — k-means + MRF segmentation, polygon vectorisation from aerial imagery

**Probabilistic Robotics**
- [FastSLAM](https://github.com/KarimAmer45/mobile-robotics-fastslam) · [EKF Localization](https://github.com/KarimAmer45/mobile-robotics-ekf-localization) · [Monte Carlo Localization](https://github.com/KarimAmer45/mobile-robotics-monte-carlo-localization) · [Occupancy Grid Mapping](https://github.com/KarimAmer45/mobile-robotics-occupancy-grid-mapping) · [Bayes Filter](https://github.com/KarimAmer45/mobile-robotics-bayes-filter) · [Odometry Motion Model](https://github.com/KarimAmer45/mobile-robotics-odometry-motion-model) · [Landmark Observation Model](https://github.com/KarimAmer45/mobile-robotics-landmark-observation-model)

**Planning & Classical CV**
- [C++ Grid Path Planner](https://github.com/KarimAmer45/cpp-grid-path-planner) · [MDP Value Iteration](https://github.com/KarimAmer45/mdp-value-iteration-planner) · [Grid Path Planning A*](https://github.com/KarimAmer45/grid-path-planning-astar)
- [Camera Calibration + Pose Demo](https://github.com/KarimAmer45/camera-calibration-pose-demo) · [Panorama Stitching](https://github.com/KarimAmer45/camera-calibration-panorama-stitching) · [Classical Image Processing](https://github.com/KarimAmer45/classical-image-processing-algorithms)
- [Graph Cut Segmentation](https://github.com/KarimAmer45/interactive-graph-cut-segmentation) · [Hough & Mean Shift](https://github.com/KarimAmer45/hough-mean-shift-segmentation) · [MOG People Tracking](https://github.com/KarimAmer45/mog-people-tracking) · [Kalman Filter Tracking](https://github.com/KarimAmer45/kalman-filter-tracking) · [Statistical Shape Modeling](https://github.com/KarimAmer45/statistical-shape-modeling)

---

## Technical Skills

**Robotics:** ROS 2, `rclcpp`, `rclpy`, `colcon`, Gazebo Sim, `nav_msgs`, `sensor_msgs`, `tf2`  
**Languages:** Python · C++17 · JavaScript · MATLAB · Bash  
**ML / Vision:** PyTorch · OpenCV · scikit-learn · Streamlit · GradCAM · SLAM  
**Infra:** Docker · Ansible · Jenkins · GitHub Actions · FastAPI  
**Hardware:** Arduino · PCB design · PLC/SCADA · embedded sensors and motor control

---

## Research Interests

- Mobile robot autonomy and field-deployable perception systems  
- Safety-aware teleoperation and human-supervised robot control  
- Sensor fusion and GNSS-denied localization  
- LLM-to-robot command interfaces  
- Multi-robot coordination  

---

## Contact

Open to research assistant roles, thesis opportunities, and robotics engineering positions involving ROS 2, perception, planning, or teleoperation.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Karim_Amer-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karim-amer-0546a2213/)
[![Email](https://img.shields.io/badge/Email-karimamer456%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:karimamer456@gmail.com)
