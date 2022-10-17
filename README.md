# planning_Gazebo_ws
Control drone by code Position + Yaw
Avoid obstacles by code Ewok

## Installation
```
git clone git@github.com:AnhDuy207/planning_Gazebo_ws.git
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
