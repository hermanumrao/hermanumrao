# Herman Singh Umrao
### Robotics Software Engineer — ROS2 Autonomous Navigation & Edge AI/Computer Vision

I build autonomous navigation stacks for ground rovers (SLAM, localization, path planning) and the embedded/edge AI systems that go with them — from sensor input to motor output. **Open to freelance and contract work** in robotics, embedded systems, and computer vision.

📧 [hermanumrao@gmail.com](mailto:hermanumrao@gmail.com) &nbsp;|&nbsp; 💼 [LinkedIn](https://linkedin.com/in/herman-singh-umrao) &nbsp;|&nbsp; 🌐 [Portfolio](https://hermanumrao.github.io/)

---

## 🛠️ What I Can Build For You

- **ROS2 navigation stacks** — SLAM (FAST-LIO, SAM-LIO, Cartographer, slam_toolbox, ORB-SLAM), localization (NDT scan matching, GICP, TEASER/TEASER++), path planning (pure pursuit, Nav2), and PID control tuning
- **Drive systems** — Ackermann, 2WD/4WD skid-steer, and mecanum-wheel platforms, including support for Clearpath rovers and TurtleBot
- **Sensor integration** — LiDAR (Livox, RPLiDAR, ST/STM32 LDx series), depth cameras (ZED, RealSense), monocular depth estimation, mmWave and UWB ranging/positioning, Pi Cam
- **Embedded firmware** — ESP32 (incl. ESP32-CSI) and STM32 (STM32CubeIDE/CubeMX) firmware for motor control, sensor telemetry, and wireless robot control; FTDI/serial bring-up
- **Simulation & data tooling** — NVIDIA Isaac Sim, Gazebo, RTAB-Map and CloudCompare for point-cloud inspection/processing
- **Computer vision pipelines** — detection, tracking, and recognition models, including edge-deployment-ready (TensorFlow Lite/ONNX) versions, deployable on Jetson or Raspberry Pi
- **Drone systems** — ArduPilot-based flight stacks, custom motor/ESC test benches, and drone hardware integration
- **Hardware build-out** — breadboard/perfboard prototyping, battery management and monitoring circuits, FDM 3D-printed enclosures and mechanical parts
- **Rapid prototyping** — proven track record of going from idea to working hardware prototype in 1–2 days (see ESP32 DeskBot below)

If your project touches any of the above, [let's talk](mailto:hermanumrao@gmail.com).

---

## 🤖 Featured Projects

### [Reloc3D-ROS2](https://github.com/hermanumrao/Reloc3D-ROS2_V1)
A ROS2 Humble package that recovers a rover's global position from a 3D LiDAR scan with no prior pose estimate — combines TEASER++ for global registration with GICP for continuous scan-to-map refinement. Drops directly into a FAST-LIO odometry pipeline and integrates with Nav2 via proper TF fusion. Handles sparse, non-uniform scans (e.g. Livox MID-360) that trip up naive ICP approaches.

### [ESP32 DeskBot](https://github.com/hermanumrao/ESP32_deskbot)
Concept-to-working-hardware in **under 15 hours**: an autonomous desk robot with ToF-based obstacle avoidance, live IMU/LiDAR telemetry over WebSocket and UDP, and phone-browser teleop with zero app install. A good reference for how fast I can turn around a self-contained embedded prototype.

### [face_detection-recognition](https://github.com/hermanumrao/face_detection-recognition)
A full face-detection/tracking pipeline built end-to-end: custom dataset capture and labeling, augmentation, and a VGG16-based dual-head model (classification + bounding-box regression) trained with a hand-written Keras training loop, running live off webcam input. Demonstrates the full CV pipeline a client project would need — not just a pretrained model wrapped in a script.

### [localization-via-slam](https://github.com/hermanumrao/localization-via-slam)
A set of production-oriented SLAM tools: a custom occupancy-grid mapper that drops the strict TF-tree requirement of `slam_toolbox`, a PCL-to-LaserScan converter, and a pose-estimation model trained directly on filtered LiDAR scans.

### [VectorDB-words](https://github.com/hermanumrao/VectorDB-words)
A vector database for word embeddings built from scratch in C++ with minimal dependencies, including an in-house GloVe-style embedding model — shows comfort working below the framework layer when performance or control matters.

---

## 🧩 More Projects

**ROS2 / Autonomy stack** — [ros2_ackermann_path_planner](https://github.com/hermanumrao/ros2_ackermann_path_planner) (hybrid A* planner for Ackermann steering), [ros2_ackermann_to_motor](https://github.com/hermanumrao/ros2_ackermann_to_motor) & [ros2_ackermann_motor_ctrl](https://github.com/hermanumrao/ros2_ackermann_motor_ctrl) (Ackermann drive commands → Arduino Mega over serial), [ros2_ackermann_keyboard_teleop](https://github.com/hermanumrao/ros2_ackermann_keyboard_teleop), [ROS2_pcd_to_occupancy_grid](https://github.com/hermanumrao/ROS2_pcd_to_occupancy_grid), [3d-mapping-rover](https://github.com/hermanumrao/3d-mapping-rover) (FAST-LIO + Livox), [wormhole_nav](https://github.com/hermanumrao/wormhole_nav) (multi-map navigation with SQL-backed room transitions), [realsense_LFR_ackermann](https://github.com/hermanumrao/realsense_LFR_ackermann) (RealSense line-follower for warehouse automation), [Qt_turtlebot_relocalizer](https://github.com/hermanumrao/Qt_turtlebot_relocalizer) (PyQt dashboard for live relocalization telemetry), [Autnomous-nav-DOCS](https://github.com/hermanumrao/Autnomous-nav-DOCS)

**Computer Vision** — [openCV_projects_cpp](https://github.com/hermanumrao/openCV_projects_cpp), [openCV_projects_python](https://github.com/hermanumrao/openCV_projects_python)

**Hardware / Embedded** — [arduino-files](https://github.com/hermanumrao/arduino-files) (drone lift mechanisms, BLDC/ESC testing, RC car + LiDAR), [edgeAI-cctv](https://github.com/hermanumrao/edgeAI-cctv) (capstone project: edge-AI inference on CCTV feeds)

**AI/ML fundamentals** — [neural-network](https://github.com/hermanumrao/neural-network), [simple-XOR-perceptron](https://github.com/hermanumrao/simple-XOR-perceptron), [text_completion_NLP](https://github.com/hermanumrao/text_completion_NLP), [pyTorch-cpp-Tutorials](https://github.com/hermanumrao/pyTorch-cpp-Tutorials), [Verilog MIPS processor](https://github.com/hermanumrao/Verilog)

**Other** — [water_suply_management](https://github.com/hermanumrao/water_suply_management) (Flask + SQLite), [phonebook](https://github.com/hermanumrao/phonebook) (trie-based, team project), [code_templates](https://github.com/hermanumrao/code_templates), [dot-config](https://github.com/hermanumrao/dot-config), [Rust_simple](https://github.com/hermanumrao/Rust_simple), [c-tutorial](https://github.com/hermanumrao/c-tutorial)

---

## 💻 Tech Stack
![C](https://img.shields.io/badge/c-%2300599C.svg?style=plastic&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=plastic&logo=c%2B%2B&logoColor=white) ![Python](https://img.shields.io/badge/python-3670A0?style=plastic&logo=python&logoColor=ffdd54) ![Rust](https://img.shields.io/badge/rust-%23000000.svg?style=plastic&logo=rust&logoColor=white) ![ROS](https://img.shields.io/badge/ROS-%2322314E.svg?style=plastic&logo=ros&logoColor=white) ![NVIDIA](https://img.shields.io/badge/NVIDIA%20Jetson-76B900.svg?style=plastic&logo=nvidia&logoColor=white) ![Raspberry Pi](https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=plastic&logo=Raspberry-Pi) ![OpenCV](https://img.shields.io/badge/opencv-%23white.svg?style=plastic&logo=opencv&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=plastic&logo=TensorFlow&logoColor=white) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=plastic&logo=PyTorch&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=plastic&logo=Keras&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=plastic&logo=scikit-learn&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=plastic&logo=numpy&logoColor=white) ![Arduino](https://img.shields.io/badge/-Arduino-00979D?style=plastic&logo=Arduino&logoColor=white) ![STMicroelectronics](https://img.shields.io/badge/STM32-03234B.svg?style=plastic&logo=stmicroelectronics&logoColor=white) ![Qt](https://img.shields.io/badge/Qt-%23217346.svg?style=plastic&logo=qt&logoColor=white) ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=plastic&logo=docker&logoColor=white) ![CMake](https://img.shields.io/badge/CMake-%23008FBA.svg?style=plastic&logo=cmake&logoColor=white) ![Flask](https://img.shields.io/badge/flask-%23000.svg?style=plastic&logo=flask&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/postgres-%23316192.svg?style=plastic&logo=postgresql&logoColor=white) ![MongoDB](https://img.shields.io/badge/MongoDB-%234ea94b.svg?style=plastic&logo=mongodb&logoColor=white) ![Linux](https://img.shields.io/badge/linux-%23FCC624.svg?style=plastic&logo=linux&logoColor=black)

**Robotics & Autonomy:** ROS2 · Nav2 · Pure Pursuit · PID Control · Ackermann / 2WD / 4WD Skid-Steer / Mecanum Drive · TurtleBot · Clearpath Rovers· FDM 3D printing

**SLAM & Localization:** FAST-LIO · SAM-LIO · Cartographer · slam_toolbox · ORB-SLAM · RTAB-Map · NDT Scan Matching · GICP · TEASER / TEASER++ · CloudCompare

**Sensors:** Livox, RPLiDAR & STM32 LDx-series LiDAR · ZED & RealSense depth cameras · Monocular depth perception · Pi Cam · mmWave · UWB

**Embedded & Hardware:** ESP32 (ESP-IDF, ESP32-CSI) · STM32 (STM32CubeIDE/CubeMX) · FTDI/serial bring-up · Breadboard & perfboard prototyping · Battery management & monitoring circuits

**Drones :** ArduPilot · Jetson · Custom drone motor/ESC test benches . delivery drones . agri-drones

**CAD/Sim:** FreeCAD . Blender . RViz2 . Gazebo . Nvidia ROS stack

---

![](https://github-readme-stats.vercel.app/api?username=hermanumrao&theme=city_lights&hide_border=false&include_all_commits=true&count_private=true)<br/>
![](https://github-readme-streak-stats.herokuapp.com/?user=hermanumrao&theme=city_lights&hide_border=false)<br/>
![](https://github-readme-stats.vercel.app/api/top-langs/?username=hermanumrao&theme=city_lights&hide_border=false&include_all_commits=true&count_private=true&layout=compact)

---

[![](https://komarev.com/ghpvc/?username=hermanumrao&label=Profile%20Views&color=0e75b6&style=flat)](https://github.com/hermanumrao)
