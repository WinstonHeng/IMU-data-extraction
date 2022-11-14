# IMU-data-extraction
This package contains 3 codes that pertain to IMU data extraction,

The first code is: sinusoidalXAccel

This code is a motion generator for a basic husky. It provides a x-acceleration in a sinusoidal waveform to the husky.


The second code is: AccelErrorServer

This code is the server for IMU data extraction service.

The third code is: AccelErrorClient

This code is the service call for IMU data extraction service.

Please first run "rosrun husky_gazebo husky_empty_world.launch" to launch a husky in a gazebo to view the husky motion.
Afterwards, run the motion generator node "rosrun imu_data_extraction sinusoidalXAccel"

Then run the server and client "rosrun imu_data_extraction AccelErrorServer" and "rosrun imu_data_extraction AccelErrorClient".

The client should provide the input that we have given to the husky, what the husky is experiencing from the IMU, and the error between the two.
