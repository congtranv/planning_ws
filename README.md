# planning_Gazebo_ws
`*` Control drone by code Position + Yaw <br>
`*` Avoid obstacles by code Ewok <br>

## Installation
```
mkdir catkin_ws
cd catkin_ws
git clone git@github.com:AnhDuy207/planning_Gazebo_ws.git src
catkin init
catkin config --extend /opt/ros/noetic
catkin config --cmake-args -DCMAKE_BUILD_TYPE=Release
catkin config --merge-devel
catkin build
```

## Getting started
1. Launch a quadrotor with px4 and mavros in gazebo 
```
roslaunch px4 mavros_posix_sitl.launch 
```
2. Run code Ewok create map
```
roslaunch ewok_optimization optimization_point.launch 
```
3. Run the offboard_position_yaw_control
```
roslaunch offboard planner.launch simulation:=true 
```
