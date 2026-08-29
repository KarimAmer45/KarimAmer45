<div align="center">

# Karim Amer

**M.Sc. Mobile Robotics · Physical AI · Robot Learning · Simulation · 3D Vision · C++ / Python**

Building reproducible robotics and perception systems: high-throughput simulation, sim-to-sim transfer, 6D pose evaluation, video object detection, sensor fusion, and safety.

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


</div>

---

## Benchmarks at a Glance

Measured results and verified behaviors are linked to reproducible commands and committed artifacts in each repository.

| Project | What was measured or verified | Result |
|---|---|:---:|
| [C++ / MuJoCo Sim-to-Sim](https://github.com/KarimAmer45/cpp-gym-nav) | Same trained PPO policy · 100 held-out seeds · randomized domain · C++ kinematics vs. MuJoCo rigid-body contact | **Randomized: 43% → 55% success · 32% → 8% collision** |
| [ROS 2–Unity Digital Twin](https://github.com/KarimAmer45/safety-aware-ros2-unity-digital-twin) | Live Gazebo → ROS 2 → Unity telemetry and deterministic safety watchdog | **28–30 Hz odom · 20 Hz safety status · ≤0.55 s stop bound** |
| [BOP 6-DoF Pose Evaluation](https://github.com/KarimAmer45/bop-6d-pose-evaluation) | Deterministic LM-O RGB-D subset · FPFH + RANSAC + ICP · 391 instances | **0.3657 ADD(-S) recall · 0.5314 AUC · 467.90 ms** |
| [LLM → ROS 2 Agent](https://github.com/KarimAmer45/llm_to_ros) | Natural-language goal → schema validation → safety clamp → deterministic ROS 2 execution | **Tool allowlist · turtlesim + Gazebo · JSONL audit trail** |
| [ROS 2 C++ Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node) | C++ safety-filter callback · 10 M iterations · `-O2` | **40 ns · 24 M calls/sec · 5 guard layers** |

---

## Visual Results

<table>
<tr>
<td align="center" width="50%">

**[C++ / MuJoCo Sim-to-Sim Transfer](https://github.com/KarimAmer45/cpp-gym-nav)**

The same seeded navigation task runs in a fast C++ kinematic backend and MuJoCo rigid-body simulation. A checked-in 100-seed transfer run exposes the success and collision gap directly.

![C++ and MuJoCo transfer on the same seeded navigation task](https://raw.githubusercontent.com/KarimAmer45/cpp-gym-nav/master/assets/generated/sim-to-sim/transfer_trained_cpp.gif)

</td>
<td align="center" width="50%">

**[Safety-Aware ROS 2–Unity Digital Twin](https://github.com/KarimAmer45/safety-aware-ros2-unity-digital-twin)**

Gazebo drives the TurtleBot3 while Unity mirrors pose and lidar. A deterministic supervisor demonstrates obstacle stops, frozen-scan handling, and operator e-stop behavior.

![Gazebo and Unity digital-twin demonstration](https://raw.githubusercontent.com/KarimAmer45/safety-aware-ros2-unity-digital-twin/main/docs/demo.gif)

</td>
</tr>
<tr>
<td align="center" width="50%">

**[BOP 6-DoF Pose Evaluation](https://github.com/KarimAmer45/bop-6d-pose-evaluation)**

Reproducible LM-O RGB-D evaluation with native ADD/ADD-S metrics, a classical FPFH–RANSAC–ICP baseline, failure accounting, and committed reports.

![BOP LM-O pose-error distributions](https://raw.githubusercontent.com/KarimAmer45/bop-6d-pose-evaluation/main/docs/results/lmo_cpu_windows_2026-08-12/error_distributions.png)

</td>
<td align="center" width="50%">

**[LLM → ROS 2 Command Interface](https://github.com/KarimAmer45/llm_to_ros)**

A tool-calling agent translates operator intent into allowlisted, schema-validated, safety-clamped ROS 2 actions across turtlesim and Gazebo backends.

![LLM to ROS command demonstration](https://raw.githubusercontent.com/KarimAmer45/llm_to_ros/main/docs/demo.gif)

</td>
</tr>
<tr>
<td align="center" colspan="2">

**[ROS 2 C++ Teleoperation Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node)**

Five independent C++ guard layers—velocity clamp, acceleration limit, deadman timeout, e-stop, and obstacle stop—running live in Gazebo Sim.

<img src="https://raw.githubusercontent.com/KarimAmer45/ros2-cpp-teleop-safety-node/main/docs/demo.gif" alt="ROS 2 C++ safety-node demonstration" width="70%">

</td>
</tr>
</table>

---

## Selected Projects

> These are the strongest end-to-end systems and measured benchmarks; the `mobile-robotics-*` algorithm studies are grouped farther down.

| | Project | Highlights |
|---|---|---|
| 🔵 | **[C++ / MuJoCo Navigation](https://github.com/KarimAmer45/cpp-gym-nav)** | C++17 + pybind11 + Gymnasium · PPO · 860k steps/s native batch · domain randomization · sim-to-sim transfer |
| 🔵 | **[Safety-Aware ROS 2–Unity Digital Twin](https://github.com/KarimAmer45/safety-aware-ros2-unity-digital-twin)** | ROS 2 + Unity + Gazebo · C# · lidar fault injection · deterministic safety supervision · 16/16 tests |
| 🔵 | **[BOP 6-DoF Pose Benchmark](https://github.com/KarimAmer45/bop-6d-pose-evaluation)** | BOP/LM-O RGB-D harness · ADD/ADD-S · FPFH + RANSAC + ICP · deterministic reports · Docker + CI |
| 🔵 | **[LLM → ROS 2 Command Interface](https://github.com/KarimAmer45/llm_to_ros)** | Tool-calling · safety clamp · schema validation · JSONL logging · turtlesim + Gazebo |
| 🔵 | **[ROS 2 C++ Teleoperation Safety Node](https://github.com/KarimAmer45/ros2-cpp-teleop-safety-node)** | 5 guard layers · 40 ns callback · CMake · CI · Gazebo Sim · 11 YAML params |
| 🔵 | **[BuzzSet YOLOV++](https://github.com/KarimAmer45/BuzzSet-org-videos)** | 4-class pollinator video detection · YOLOV++ temporal pipeline · YOLOX-Swin · RF-DETR comparison · COCO AP |
| 🔵 | **[NavViz Unreal](https://github.com/KarimAmer45/navviz-unreal)** | Unreal Engine 5 C++ renderer · PPO world-state streaming over TCP/JSON · real-time 3D visualization |
| 🔵 | **[GNSS-Denied Visual-Inertial Localization](https://github.com/KarimAmer45/gnss-denied-visual-inertial-localization)** | EKF sensor fusion · Docker · ROS 2 C++ wrapper · regression tests · 0.24 m outage RMSE |
| 🔵 | **[Explainable Vision Demo](https://github.com/KarimAmer45/explainable-vision-demo)** | ResNet · EfficientNet · ViT · GradCAM · attention rollout · 3 Streamlit apps · CI |

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

**Simulation & Physical AI:** MuJoCo, Gymnasium, Gazebo, Unity, Unreal Engine, PPO, domain randomization, sim-to-sim transfer, reduced-order modeling  
**Robotics:** ROS 2, `rclcpp`, `rclpy`, `colcon`, `nav_msgs`, `sensor_msgs`, `tf2`  
**Languages:** Python, C++17, C#, JavaScript, MATLAB, Bash  
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

Open to research assistant, thesis, and robotics engineering opportunities in Physical AI, robot learning, simulation, perception, and safety-aware autonomy.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Karim_Amer-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/karim-amer-0546a2213/)
[![Email](https://img.shields.io/badge/Email-karimamer456%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:karimamer456@gmail.com)