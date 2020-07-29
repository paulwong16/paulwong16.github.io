---
layout: archive
title: "Selected Projects"
permalink: /projects/
author_profile: true
---

{% include base_path %}

# Comparison on fusion-based single image HDR enhancement #

Assigned to ECE 613 Project.

<a href="https://github.com/paulwong16/ldr2hdr"><i class="fas fa-external-link-alt" aria-hidden="true"></i>Source Code</a>

# Odom-Laser Calibration Tool #

Copyright Megvii Technology Ltd. 

<img src="http://paulwong16.github.io/files/calibration.png" alt="calibration_tool" width="800"/>

Here we implemented a easy-use tool for following parameters' calibration: yaw-rotation and xy-translation between odom and 2D-LiDAR, and radius of odom's wheels and axle between them. For more details and usage please reference to our project's page.

For Chinese version introduction please reference to homepage of my colleague <a href="https://blog.csdn.net/heyijia0327/article/details/88571176">Dr. Yijia He</a>.

- References: Censi, Andrea, Franchi, Antonio, Marchionni, Luca & Oriolo, Giuseppe (2013). Simultaneous calibration of odometry and sensor parameters for mobile robots. IEEE Transactions on Robotics, 29, 475-492.

<a href="https://github.com/MegviiRobot/OdomLaserCalibraTool"><i class="fas fa-external-link-alt" aria-hidden="true"></i>Source Code</a>

# Continuous Localization and Mapping in low-light GPS-denied Environments #

We propose a system for simultaneous localization and mapping in low-light environments based on multi-sensors fusion. Thermal Visual Odometry in our approach is obtained from a thermal camera’s multi-plane Homography decomposition with IMU Pose and laser altitude, and optimized by a Kalman Filter. In addition, based on multi-layers Grid Map, our system can create a robot-centric map fused by multi-plane extraction and laser scanner measurement.

<img src="http://paulwong16.github.io/files/fig1.png" alt="overview" width="400"/>

<img src="http://paulwong16.github.io/files/fig3(1).png" alt="plane detection 1" width="400"/>

<img src="http://paulwong16.github.io/files/fig3(2).png" alt="plane detection 2" width="400"/>

<img src="http://paulwong16.github.io/files/fig9.png" alt="grid map" width="400"/>

<img src="http://paulwong16.github.io/files/fig9-all.png" alt="landing point detection" width="1200"/>

**Zhijie Wang**, Yingcai Bi, Ben M. Chen, Continuous Localization and Mapping for Autonomous Navigation in low-light environments based on Multi-Sensors Fusion, *IEEE International Conference on Control and Automation*.

<a href="https://github.com/paulwong16/TVO-GridMap"><i class="fas fa-external-link-alt" aria-hidden="true"></i>Coming Soon</a>


# Underwater Image Enhancer #

We propose a novel architecture that can jointly extract local features and global features and elegantly fuse them together to perform underwater image enhancement based on the framework of conditional generative adversarial networks (cGANs) with residual blocks. The network is trained in an end-to-end fashion. Our approach is validated with subjective and objective tests and comparison against the state of the art, where we show great improvements.

Xiaodong Liu, Zhi Gao, **Zhijie Wang**, Yu Herng Tan, Yingcai Bi, Ben M. Chen, Underwater Image Enhancer based on Conditional GANs, *IEEE Transactions on Circuits and Systems for Video Technology.*.


<iframe width="560" height="315" src="https://www.youtube.com/embed/c1mKxQCx_24" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<iframe width="560" height="315" src="https://www.youtube.com/embed/hMVFj03pVUQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>


<a href="https://github.com/Xiaodong-Bran/underwater-image-enhancer"><i class="fas fa-external-link-alt" aria-hidden="true"></i>Coming Soon</a>
