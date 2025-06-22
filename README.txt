source /opt/ros/jazzy/setup.bash
cd dev_ws
colcon build --symlink-install

publish voor rviz2
ros2 launch my_bot rsp.launch.py

run gazebo
ros2 launch my_bot launch_sim.launch.py  

pushish voor gazebo
ros2 launch my_bot rsp.launch.py use_sim_time:=true       

