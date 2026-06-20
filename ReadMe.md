# 🤖 Hi, I'm Herman Singh Umrao 👋
### **Robotics Software Engineer — ROS2 Autonomous Navigation & Edge AI/Computer Vision**

<p align="left">
  <a href="mailto:hermanumrao@gmail.com"><img src="https://img.shields.io/badge/Email-hermanumrao%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://linkedin.com/in/herman-singh-umrao"><img src="https://img.shields.io/badge/LinkedIn-Herman%20Singh%20Umrao-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <a href="https://hermanumrao.github.io/"><img src="https://img.shields.io/badge/Portfolio-hermanumrao.github.io-0055FF?style=for-the-badge&logo=firefoxbrowser&logoColor=white"/></a>
</p>

I build autonomous navigation stacks for ground rovers (SLAM, localization, path planning) and the embedded/edge AI systems that go with them — from sensor input to motor output. 

⚙️ **Available for Freelance & Contract Work** in robotics hardware/software architecture, embedded systems, and machine vision.

---

## ⚡ What I Can Build For You

<details open>
<summary>🛠️ <b>Autonomy, Navigation & Drive Systems</b></summary>
<br>

- **ROS2 Navigation Stacks:** Complete integration of SLAM (`FAST-LIO`, `SAM-LIO`, `Cartographer`, `slam_toolbox`, `ORB-SLAM`), point-cloud localization (`NDT scan matching`, `GICP`, `TEASER/TEASER++`), path planning (`Nav2`, `pure pursuit`), and precision PID control tuning.
- **Drive Kinematics:** Custom drive system configurations for **Ackermann steering, 2WD/4WD skid-steer, and Mecanum-wheel platforms**. Experienced with Clearpath rovers and TurtleBot ecosystems.
- **Simulation & Point-Clouds:** Virtual environment configurations via `NVIDIA Isaac Sim` and `Gazebo`; post-processing with `RTAB-Map` and `CloudCompare`.
</details>

<details open>
<summary>🔌 <b>Embedded Firmware & Sensor Integration</b></summary>
<br>

- **Sensors:** Dense/sparse LiDAR arrays (`Livox MID-360`, `RPLiDAR`, `ST/STM32 LDx series`), stereoscopic/depth vision (`ZED`, `RealSense`), monocular depth estimation network deployment, `mmWave` & `UWB` spatial ranging.
- **Firmware:** Custom `ESP32` (including `ESP32-CSI` tracking) and `STM32` (`STM32CubeIDE/CubeMX`) code bases written for low-latency motor control, custom sensor telemetry parsing, and radio-link configurations.
</details>

<details open>
<summary>👁️ <b>Edge AI, Drones & Rapid Hardware Prototyping</b></summary>
<br>

- **Computer Vision:** End-to-end perception pipelines (object detection, spatial tracking, feature recognition) compiled into edge-friendly runtimes (`TensorFlow Lite`, `ONNX`) for deployment on `Nvidia Jetson` or `Raspberry Pi`.
- **Aviation:** `ArduPilot`-based flight stack setups, payload mechanics, customized motor/ESC dynamometer test benches, and structural integration for specialized delivery and agricultural drones.
- **Hardware Integration:** Speed-optimized breadboard/perfboard electrical prototyping, custom battery management system (BMS) logic, and robust `FDM 3D-printed` custom structural enclosures. **Proven runtime optimization:** going from raw idea to fully functional hardware prototype inside 24 hours.
</details>

---

## 🚀 Featured Projects

### 📡 [Reloc3D-ROS2](https://github.com/hermanumrao/Reloc3D-ROS2_V1)
> **Global 3D LiDAR Relocalization package for ROS2 Humble.**
- Recovers global coordinates without a prior pose estimate by executing a robust correspondence-free global registration (`TEASER++`) combined with sequential iterative closest point adjustment (`GICP`).
- Plugs directly into standard `FAST-LIO` pipelines and broadcasts correct coordinate updates to `Nav2` via proper TF fusion.
- Built to handle sparse, non-uniform spatial scans (e.g., `Livox MID-360`) that typical naive point-matching frameworks fail to resolve.

### 🏎️ [ESP32 DeskBot](https://github.com/hermanumrao/ESP32_deskbot)
> **Fully autonomous micro-rover turned around from concept to operating hardware in under 15 hours.**
- Integrates time-of-flight (ToF) obstacle collision avoidance and publishes live IMU/LiDAR telemetry matrices via concurrent `WebSocket` and `UDP` streams.
- Provides an instantly accessible browser-based mobile controller dashboard requiring zero client app installation. 

### 👁️ [Face Detection & Tracking Pipeline](https://github.com/hermanumrao/face_detection-recognition)
> **An end-to-end computer vision tracking system optimized for live processing.**
- Built from raw framework layer up: proprietary training-set capture routines, structural dataset data augmentation, and a dual-headed `VGG16` network topology configured for concurrent classification and coordinate bounding-box regression.
- Utilizes a purely hand-written custom Keras training loop running dynamic inference pipelines live over raw webcam streams.

### 🗺️ [Localization via SLAM](https://github.com/hermanumrao/localization-via-slam)
> **Production-ready standalone spatial mapping and odometry toolkit.**
- Features a proprietary occupancy-grid calculation pipeline designed to drop strict structural TF-tree constraints typically requested by standard `slam_toolbox`.
- Includes efficient `PCL-to-LaserScan` conversion utilities and a structural pose estimation model trained directly on filtered, downsampled raw LiDAR scans.

### 🗄️ [VectorDB-Words](https://github.com/hermanumrao/VectorDB-words)
> **High-performance minimalist vector database engine engineered from scratch in native C++.**
- Zero massive external framework dependencies; includes an in-house engineered word embedding model optimized for memory constraints. Designed for applications where sub-framework compute control is required.

---

## 🧩 Additional Repository Index

<div align="left">
  <table>
    <tr>
      <td><b>🤖 Autonomy & Controls</b></td>
      <td>
        • <a href="https://github.com/hermanumrao/ros2_ackermann_path_planner">ros2_ackermann_path_planner</a> — Hybrid A* path planning for car-like chassis.<br>
        • <a href="https://github.com/hermanumrao/ros2_ackermann_to_motor">ros2_ackermann_to_motor</a> — Translation engine parsing commands to hardware.<br>
        • <a href="https://github.com/hermanumrao/ros2_ackermann_motor_ctrl">ros2_ackermann_motor_ctrl</a> — Serial motor bridge running over Arduino Mega.<br>
        • <a href="https://github.com/hermanumrao/ros2_ackermann_keyboard_teleop">ros2_ackermann_keyboard_teleop</a> — Custom keyboard validation layouts.<br>
        • <a href="https://github.com/hermanumrao/ROS2_pcd_to_occupancy_grid">ROS2_pcd_to_occupancy_grid</a> — Automated point-cloud projection engine.<br>
        • <a href="https://github.com/hermanumrao/3d-mapping-rover">3d-mapping-rover</a> — Portable mapping rig using FAST-LIO & Livox hardware.<br>
        • <a href="https://github.com/hermanumrao/wormhole_nav">wormhole_nav</a> — Multi-map transit transitions tracking via SQL data engines.<br>
        • <a href="https://github.com/hermanumrao/realsense_LFR_ackermann">realsense_LFR_ackermann</a> — RealSense vision-based line tracking for AGVs.<br>
        • <a href="https://github.com/hermanumrao/Qt_turtlebot_relocalizer">Qt_turtlebot_relocalizer</a> — Performance PyQt console dashboard tracking odometry.<br>
        • <a href="https://github.com/hermanumrao/Autnomous-nav-DOCS">Autnomous-nav-DOCS</a> — Core autonomy engineering notes & setup scripts.
      </td>
    </tr>
    <tr>
      <td><b>💻 Vision & Embeds</b></td>
      <td>
        • <a href="https://github.com/hermanumrao/openCV_projects_cpp">openCV_projects_cpp</a> / <a href="https://github.com/hermanumrao/openCV_projects_python">openCV_projects_python</a> — Low-latency computer vision routines.<br>
        • <a href="https://github.com/hermanumrao/arduino-files">arduino-files</a> — Custom firmware scripts for BLDC/ESC benches, drone lift structures, and RC conversions.<br>
        • <a href="https://github.com/hermanumrao/edgeAI-cctv">edgeAI-cctv</a> — Capstone deployment: Low-power edge neural network inferencing over CCTV stream grids.
      </td>
    </tr>
    <tr>
      <td><b>🧠 Core Foundations</b></td>
      <td>
        • <a href="https://github.com/hermanumrao/neural-network">neural-network</a> — Forward/backward mathematical propagation engines in raw matrices.<br>
        • <a href="https://github.com/hermanumrao/simple-XOR-perceptron">simple-XOR-perceptron</a> — Fundamental classification mathematical checks.<br>
        • <a href="https://github.com/hermanumrao/text_completion_NLP">text_completion_NLP</a> — Minimal NLP word matrix sequencer.<br>
        • <a href="https://github.com/hermanumrao/pyTorch-cpp-Tutorials">pyTorch-cpp-Tutorials</a> — High-performance execution configurations using libtorch C++ bindings.<br>
        • <a href="https://github.com/hermanumrao/Verilog">Verilog MIPS Processor</a> — Hardware descriptive logic verification for computing cores.
      </td>
    </tr>
    <tr>
      <td><b>⚡ Other Projects</b></td>
      <td>
        • <a href="https://github.com/hermanumrao/water_suply_management">water_suply_management</a> — Flask structural tracker back-ended via SQLite.<br>
        • <a href="https://github.com/hermanumrao/phonebook">phonebook</a> — High-efficiency trie-based lookup tracking array structure.<br>
        • <a href="https://github.com/hermanumrao/code_templates">code_templates</a> / <a href="https://github.com/hermanumrao/dot-config">dot-config</a> — My Arch Linux daily driver setup environment dots.<br>
        • <a href="https://github.com/hermanumrao/Rust_simple">Rust_simple</a> / <a href="https://github.com/hermanumrao/c-tutorial">c-tutorial</a> — Language specific syntax engineering trackers.
      </td>
    </tr>
  </table>
</div>

---

## 💻 Technical Infrastructure Stack

### **Core Tooling & Runtimes**
<p align="left">
  <img src="https://img.shields.io/badge/c-%2300599C.svg?style=flat-square&logo=c&logoColor=white" alt="C"/>
  <img src="https://img.shields.io/badge/c++-%2300599C.svg?style=flat-square&logo=c%2B%2B&logoColor=white" alt="C++"/>
  <img src="https://img.shields.io/badge/python-3670A0?style=flat-square&logo=python&logoColor=ffdd54" alt="Python"/>
  <img src="https://img.shields.io/badge/rust-%23000000.svg?style=flat-square&logo=rust&logoColor=white" alt="Rust"/>
  <img src="https://img.shields.io/badge/ROS2-%2322314E.svg?style=flat-square&logo=ros&logoColor=white" alt="ROS2"/>
  <img src="https://img.shields.io/badge/NVIDIA%20Jetson-76B900.svg?style=flat-square&logo=nvidia&logoColor=white" alt="NVIDIA Jetson"/>
  <img src="https://img.shields.io/badge/-Raspberry_Pi-C51A4A?style=flat-square&logo=Raspberry-Pi" alt="Raspberry Pi"/>
  <img src="https://img.shields.io/badge/opencv-%23white.svg?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV"/>
  <img src="https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=flat-square&logo=TensorFlow&logoColor=white" alt="TensorFlow"/>
  <img src="https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=flat-square&logo=PyTorch&logoColor=white" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=Arduino&logoColor=white" alt="Arduino"/>
  <img src="https://img.shields.io/badge/STM32-03234B.svg?style=flat-square&logo=stmicroelectronics&logoColor=white" alt="STM32"/>
  <img src="https://img.shields.io/badge/Docker-%230db7ed.svg?style=flat-square&logo=docker&logoColor=white" alt="Docker"/>
  <img src="https://img.shields.io/badge/CMake-%23008FBA.svg?style=flat-square&logo=cmake&logoColor=white" alt="CMake"/>
  <img src="https://img.shields.io/badge/Linux-%23FCC624.svg?style=flat-square&logo=linux&logoColor=black" alt="Linux"/>
</p>

### **Architecture Specializations Breakdown**
* **Robotics & Control Autonomy:** Nav2 Architecture • Pure Pursuit Mathematics • PID Gain Tuning Loops • Kinematic Matrices (Ackermann / Skid-Steer / Mecanum Platform Drives) • Clearpath Systems • AMRs & UAV Airframe Layouts • FDM Structural 3D Printing Production.
* **SLAM & State Estimation:** FAST-LIO / SAM-LIO Solid-State & Mechanical LiDAR Pipelines • Cartographer & slam_toolbox Map Tuning • NDT / GICP Point Registration Engines • TEASER++ Arbitrary Frame Alignments • Dense Cloud Diagnostics (`CloudCompare`).
* **Perception Array Ecosystems:** Livox Solid-State Array Systems • RPLiDAR Scanners • STM32 Custom Serial Ranging Engines • ZED & Intel RealSense Stereoscopic Depth Perception Units • FMCW mmWave Radar Sensors • Ultra-Wideband (UWB) Spatial Positioning Grids.
* **Embedded Hardware Engineering:** Custom ESP-IDF Systems • STM32 HAL & Low-Layer Low-latency Execution Pipelines • Raw Hardware Transceiver Bring-Up (FTDI, Logic Analyzers, UART/SPI/I2C diagnostics) • Custom Prototyping Power Configurations & Battery Management Units.
* **Simulation, Graphics & Data Engines:** Nvidia Isaac Sim Systems • Gazebo Classic/Harmonic Ecosystems • PyQt Desktop Control Engine Engineering • Solid SQL/NoSQL Infrastructure Arrays (`PostgreSQL`, `MongoDB`).

---

## 📊 Performance Metrics

<p align="left">
  <!-- GitHub Streak Stats -->
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=hermanumrao&theme=tokyonight&hide_border=false" alt="Herman's GitHub Streak" height="170"/>
  
  <!-- Alternative Reliable Stats Card -->
  <img src="https://github-readme-stats.vercel.app/api?username=hermanumrao&theme=tokyonight&show_icons=true&count_private=true" alt="Herman's GitHub Stats" height="170"/>
</p>


## 🏆 GitHub Trophies

[![trophy](https://github-trophies.vercel.app/?username=hermanumrao&theme=onedark)](https://github.com/lucthienphong1120/github-trophies)

---

<p align="center">
  <a href="https://github.com/hermanumrao">
    <img src="https://komarev.com/ghpvc/?username=hermanumrao&label=Profile%20Views&color=0e75b6&style=flat-square" alt="Profile Views"/>
  </a>
</p>
