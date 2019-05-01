在gmapping下使用激光雷达进行模拟建图

1.安装GMAPPING
2.启动GMAPPING
  roslaunch gmapping slam_gmapping_hibot_rplidar_a1.launch
  一定要启动robot_state_publisher节点，发布“tf_static”话题，或以其它方式发布，
  gmapping用于建图
3.打开 rviz
  rviz -d slam_gmapping/gmapping/launch/rplidar_a1_test.rviz 配置文件
4.保存地图
  rosrun map_server map_saver -f work0
