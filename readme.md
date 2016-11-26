#Data Collection using Bebop

This is a simple code that shows application of message_filters and custom messages for a synchronized data collection.
The code works for Parrot Bebop and Bebop2 quadcopter. It can be used with AR.Drone by simply changing the topic names at appropriate places. Similarly it can be used with any other robot or camera for data collection purposes by changing the topics being subscribed to.

In this code, we are storing the msgs from camera, fix from GPS module, and odometry data from IMU of quadcopter, and ORB SLAM. ORB SLAM is a monocular slam (http://webdiis.unizar.es/~raulmur/orbslam/). We can store additional data or remove some of the mentioned data by changing the subscriber nodes and message_filter definition.

Clone the repo in ros workspace and do 'catkin_make --pkg bebop_data' to build. Will have to set the path to folder where images are to be stored.
