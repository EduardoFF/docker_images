# This is an auto generated Dockerfile for ros:kinetic-ros-base
# generated from templates/docker_images/create_ros_image.Dockerfile.em
# generated on 2017-01-27 02:34:03 +0000
FROM jeguzzi/ros:armhf-melodic-ros-base

RUN apt-get update && apt-get install -y \
   git build-essential python-rosdep python-catkin-tools \
   && rm -rf /var/lib/apt/lists/*

RUN mkdir -p /root/catkin_ws/src

WORKDIR /root/catkin_ws

RUN /bin/bash -c 'source /opt/ros/melodic/setup.bash; catkin init; catkin build'

RUN /bin/sed -i \
  '/source "\/opt\/ros\/$ROS_DISTRO\/setup.bash"/a source "\/root\/catkin_ws\/devel\/setup.bash"' \
  /ros_entrypoint.sh
