# CAD Models for the Sensor Mount
We provide the CAD files for the sensor mount.
[[SLDPRT]](https://github.com/SangwooJung98/Co-RaL-Dataset/blob/main/system/single_radar_imu_spot.SLDPRT)
[[STL]](https://github.com/SangwooJung98/Co-RaL-Dataset/blob/main/system/single_radar_imu_spot.STL)

![image](https://github.com/user-attachments/assets/596de208-47a4-4619-9f11-ced8055fd68e)

# ROS1 Driver Links
### TI mmWave radar
https://github.com/hojjunekim/ti_mmwave_rospkg
- Fixed original driver's problem that it is not providing radial velocity on pointcloud (Previously, gathered 'point' topic that gives every information of each point)
### BD SPOT Driver
https://github.com/heuristicus/spot_ros
- ROS1 driver (python based)

# ROS2 Driver Links
### TI mmWave radar
https://github.com/kimsooyoung/mmwave_ti_ros
- ROS2 official driver (last commit on 3 years ago)
### microstrain IMU
https://github.com/LORD-MicroStrain/microstrain_inertial/tree/ros2
- ROS2 official driver (still updating)
### BD SPOT Driver
https://github.com/bdaiinstitute/spot_ros2?tab=readme-ov-file
- ROS2 official driver (cpp based)
