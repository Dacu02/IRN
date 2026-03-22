gazebo:
	bash -c "source /opt/ros/humble/setup.bash && \
	source install/setup.bash && \
	ros2 launch diem_gazebo turtlebot4_ignition_no_dock.launch.py world:=square"
controller:
	bash -c "source /opt/ros/rolling/setup.bash && \
	source install/setup.bash && \
	ros2 control switch_controllers --activate joint_state_broadcaster diffdrive_controller"
list_controller:
	bash -c "source /opt/ros/rolling/setup.bash && \
	source install/setup.bash && \
	ros2 control list_controllers"
debug_controller:
	bash -c "source /opt/ros/rolling/setup.bash && \
	source install/setup.bash && \
	ros2 run controller_manager ros2_control_node --ros-args --log-level controller_manager:=debug"
