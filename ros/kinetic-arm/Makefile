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
	@docker build --tag=jeguzzi/ros:armhf-kinetic-ros-core          kinetic-ros-core/.
	@docker build --tag=jeguzzi/ros:armhf-kinetic-ros-base          kinetic-ros-base/.
	@docker build --tag=jeguzzi/ros:armhf-kinetic-ros-dev           kinetic-ros-dev/.

pull:
	@docker pull jeguzzi/ros:armhf-kinetic-ros-core
	@docker pull jeguzzi/ros:armhf-kinetic-ros-base
	@docker pull jeguzzi/ros:armhf-kinetic-ros-dev

clean:
	@docker rmi -f jeguzzi/ros:armhf-kinetic-ros-core
	@docker rmi -f jeguzzi/ros:armhf-kinetic-ros-base
	@docker rmi -f jeguzzi/ros:armhf-kinetic-ros-dev

push:
	@docker push jeguzzi/ros:armhf-kinetic-ros-core
	@docker push jeguzzi/ros:armhf-kinetic-ros-base
	@docker push jeguzzi/ros:armhf-kinetic-ros-dev
