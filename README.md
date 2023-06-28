## AVG_simulation运作方式

- 打开roscore

- 运行 roslaunch AVG_simulation car.launch

- 发布 cmd_vel 话题消息控制小车运动（指令或摇杆）


## cmd发布指令控制示例

- 设置线速度和角速度 rostopic pub -r 10 /cmd_vel geometry_msgs/Twist '{linear: {x: 0.2, y: 0, z: 0}, angular: {x: 0, y: 0, z: 0.5}}'

- 指令可参考http://wiki.ros.org/arbotix


## 摇杆控制示例

- 安装对应的ros包 sudo apt install ros-noetic-rqt-robot-steering

- 运行 rosrun rqt_robot_steering rqt_robot_steering

- 用摇杆控制小车的线速度和角速度

