all: help

help:
	@echo ""
	@echo "-- Help Menu"
	@echo ""
	@echo "   1. make build            - build all images"
	@echo "   2. make pull             - pull all images"
	@echo "   3. make clean            - remove all images"
	@echo ""

build:
	@docker build --tag=jeguzzi/ros:arm64-melodic-ros-core          ros-core/.
	@docker build --tag=jeguzzi/ros:arm64-melodic-ros-base          ros-base/.
	@docker build --tag=jeguzzi/ros:arm64-melodic-ros-dev          dev/.
	# @docker build --tag=jeguzzi/ros:arm64-melodic-robot             robot/.
	# @docker build --tag=jeguzzi/ros:arm64-melodic-perception        perception/.
	# @docker build --tag=osrf/jeguzzi/ros:arm64-melodic-desktop      desktop/.
	# @docker build --tag=osrf/jeguzzi/ros:arm64-melodic-desktop-full desktop-full/.

pull:
	@docker pull jeguzzi/ros:arm64-melodic-ros-core
	@docker pull jeguzzi/ros:arm64-melodic-ros-base
	@docker pull jeguzzi/ros:arm64-melodic-ros-dev
	# @docker pull jeguzzi/ros:arm64-melodic-robot
	# @docker pull jeguzzi/ros:arm64-melodic-perception
	# @docker pull osrf/jeguzzi/ros:arm64-melodic-desktop
	# @docker pull osrf/jeguzzi/ros:arm64-melodic-desktop-full

clean:
	@docker rmi -f jeguzzi/ros:arm64-melodic-ros-core
	@docker rmi -f jeguzzi/ros:arm64-melodic-ros-base
	@docker rmi -f jeguzzi/ros:arm64-melodic-ros-dev
	# @docker rmi -f jeguzzi/ros:arm64-melodic-robot
	# @docker rmi -f jeguzzi/ros:arm64-melodic-perception
	# @docker rmi -f osrf/jeguzzi/ros:arm64-melodic-desktop
	# @docker rmi -f osrf/jeguzzi/ros:arm64-melodic-desktop-full

push:
	@docker push jeguzzi/ros:arm64-melodic-ros-core
	@docker push jeguzzi/ros:arm64-melodic-ros-base
	@docker push jeguzzi/ros:arm64-melodic-ros-dev
