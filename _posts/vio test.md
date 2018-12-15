# Tests on Two Major VIO Algorithms #

- **Test date:** July 31st.

- **Algorithms:** MSCKF-VIO & VINS-MONO

- **Environment:** UAV Lab (E4A 03-04, NUS)

- **Sensors:** 2 Point Grey Cameras (Chameleon3 2.8mm) / VN-100 IMU (adis16480)


## About ##

We test on two popular open source vio (visual-inertial odometry) algorithms, [VINS-MONO](https://github.com/HKUST-Aerial-Robotics/VINS-Mono)\[1] and [MSCKF-VIO](https://github.com/KumarRobotics/msckf_vio)\[2]. Apparently the major diference between them is the numbers of cameras, only one camera used in \[1] but two in \[2]. Accroding to the \[2]'s authors that stereo cameras could raise the performances, we did a simple test and therefore compared the results.


## Step ##

1. Install the camera and IMU drivers.

2. Implement two algorithms through their official open source ros package.

3. Calibrate the sensors.

4. Record a dataset in rosbag type.

5. Test two algorithms on the dataset.

6. Compare the results.


## Calibration ##

We use the [Kalibr](https://github.com/ethz-asl/kalibr) to calibrate the cameras and T&R matrix between cameras and imu. The results are showing below and the accurate calibration file could be downloaded [here](https://paulwon.moe).

## Notices When Test ##

- Since \[1] has the loop-closing mode that we need to turn it off.

- There is a time-delay between imu and images which is short but need to be concerned about. The authors of \[1] provide the delay calculation and we consider this delay is approximately accurate to use in \[2].

- \[1] needs a step of raising vertically and the dataset must contains some rotation or accelerating to fulfill the experiment procedure.

## Test Result ##

The test video are showing below.

We record the odometry of these two algorithms and plot them in MATLAB in the same coordinate. Fig 1 shows that after turnning off the loop-closing mode, \[1] has a drift in X-Y plane though we started and ended in the same position while the Fig 2 shows that \[2] has a bigger drift in Z.

Besides, \[2] needs more CPU resources because of the processing of stereo images. And \[1] performs not so good when pirouetting.

## References ##


\[1] Qin, Tong, Peiliang Li, and Shaojie Shen. "VINS-Mono: A robust and versatile monocular visual-inertial state estimator." IEEE Transactions on Robotics 99 (2018): 1-17.

\[2] Sun, Ke, et al. "Robust stereo visual inertial odometry for fast autonomous flight." IEEE Robotics and Automation Letters 3.2 (2018): 965-972. 
