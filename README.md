# Co-RaL-Dataset
## Co-RaL: Complementary Radar-Leg Odometry with 4-DoF Optimization and Rolling Contact

### Authors:
[Sangwoo Jung](https://sangwoojung98.github.io), [Wooseong Yang](https://rpm.snu.ac.kr) and [Ayoung Kim](https://ayoungk.github.io)*. 

## Paper and Video Link
IEEE (TBD)

[Arxiv](https://arxiv.org/abs/2407.05820)

[Youtube Video](https://youtu.be/kHKn85_KKgk)

Welcome to Co-RaL-Dataset!
This repository includes the experimental dataset acquired to evaluate our radar-leg odometry algorithm, Co-RaL, which has been accepted by IEEE IROS 2024. 
Our dataset includes sensor data of chip radar, imu, velodyne, and kinematic data from Boston Dynamics SPOT (Joint encoders and contact sensors). 
Each sequence is acquired with different environments to evaluate the algorithm performance generally. 
The dataset is provided with ROS Bag file format. 

## Download Link
[Google Drive](https://drive.google.com/drive/folders/1Sa3D52G-bcQO7JdfdrSAYSNStKwa9spB?usp=sharing)

## Sensor Setup

<div align="left">
  <img src="https://github.com/SangwooJung98/Co-RaL-Dataset/assets/48044261/96eb9d8c-b5dd-4930-9dae-d5b6a2651324" alt="photo" width="60%">
</div>

Sensor|Model|Data Type|Freq|ROS Topic
:--:|:--:|:--:|:--:|:--:
chip radar | AWR1843BOOST | 4D radar pointcloud | 20Hz | /radar_0/radarcloud_gather
IMU | 3dm-gx5-25 | 9 DoF IMU data (Acc, ang Vel, orien) | 100Hz | /imu
LiDAR | Velodyne VLP-16 | 3D LiDAR pointcloud | 10Hz | /velodyne_points
Joint Encoder | Spot Joint Sensor | 12 float values (List) | 180Hz | /joint_states
Contact Sensor | Spot Contact Sensor | 4 boolean values (List) | 180Hz | /spot/status/feet
Time | - | ROS time | - | /clock

## Dataset List

Sequence|Environment|Stair|Slope|Narrow Path|Path Length (m)|Elevation Change (m)|Duration (s)|Avg. vel. (m/s)
:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:|:--:
Stair|Outdoor|✓|✓|✗|253.24|15.12|304.40|0.832
Under|Indoor|✗|✓|✗|227.02|3.23|258.50|0.878
Narrow|Outdoor|✗|✗|✓|134.86|-|151.39|0.891
Trail|Outdoor|✗|✓|✗|230.10|11.37|253.36|0.908
Garage|Hybrid|✗|✓|✗|138.52|-|161.68|0.857
Building|Hybrid|✓|✓|✗|252.86|8.26|291.89|0.866

## Contact
This dataset is provided for academic purposes. If you encounter some technical problems, please open an issue or contact <Sangwoo Jung: dan0130@snu.ac.kr>.

## Citation
TBD
