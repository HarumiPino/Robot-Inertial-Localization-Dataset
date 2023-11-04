# Robot-Inertial-Localization-Dataset

Dataset used for paper "Indoor Mobile Robot Localization Using Machine Learning". All data was captured in simulated environments with a simulated *TurtleBot3* robot with a sampling rate of 200 Hz.
Dataset is divided into training set (train_data) and testing set (test_data). Each of these sets are futher divided into different trajectories, as follows:
1. **Training set**
	- 26 trajectories in an empty environment
	- 12 trajectories in an environment with obstacles
2. **Testing set**
	- 10 trajectories in an empty environment
	- 2 trajectories in an environment with obstacles

Each folder corresponding to each trajectory contains two files:
- **imu_data:** File containing data captured from robot IMU.
- **pose_data:** File containing the real position of the robot during data capture.

The **imu_data** file contains 41 columns containing the following information:
- %time
- field.header.seq
- field.header.stamp
- field.header.frame_id
- field.orientation.x
- field.orientation.y
- field.orientation.z
- field.orientation.w
- field.orientation_covariance0
- field.orientation_covariance1
- field.orientation_covariance2
- field.orientation_covariance3
- field.orientation_covariance4
- field.orientation_covariance5
- field.orientation_covariance6
- field.orientation_covariance7
- field.orientation_covariance8
- field.angular_velocity.x
- field.angular_velocity.y
- field.angular_velocity.z
- field.angular_velocity_covariance0
- field.angular_velocity_covariance1
- field.angular_velocity_covariance2
- field.angular_velocity_covariance3
- field.angular_velocity_covariance4
- field.angular_velocity_covariance5
- field.angular_velocity_covariance6
- field.angular_velocity_covariance7
- field.angular_velocity_covariance8
- field.linear_acceleration.x
- field.linear_acceleration.y
- field.linear_acceleration.z
- field.linear_acceleration_covariance0
- field.linear_acceleration_covariance1
- field.linear_acceleration_covariance2
- field.linear_acceleration_covariance3
- field.linear_acceleration_covariance4
- field.linear_acceleration_covariance5
- field.linear_acceleration_covariance6
- field.linear_acceleration_covariance7
- field.linear_acceleration_covariance8

The **pose_data** file contains 3 columns containing the following information:
- %time
- poseX
- poseY
