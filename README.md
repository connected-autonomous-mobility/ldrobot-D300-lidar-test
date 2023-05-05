# ldrobot-D300-lidar-test
testing lidar https://www.ldrobot.com/product/en/126

[README](https://github.com/ldrobotSensorTeam/DeveloperKit/blob/master/D300Kit.md)




## 1 sdk
```
rainer@jetsonautoware46:~/projects/ldlidar_stl_sdk/build$ 
./ldlidar_stl /dev/ttyUSB0
```
```
[ldrobot] angle: 332.97 distance(mm): 684 intensity: 235 
[ldrobot] angle: 333.84 distance(mm): 824 intensity: 232 
[ldrobot] angle: 334.71 distance(mm): 839 intensity: 233 
[ldrobot] angle: 335.58 distance(mm): 839 intensity: 235 
[ldrobot] angle: 336.45 distance(mm): 839 intensity: 233 
[ldrobot] angle: 337.32 distance(mm): 855 intensity: 231 
[ldrobot] angle: 338.19 distance(mm): 855 intensity: 232 
```

## 2 ros - rviz
[install ros package](https://github.com/ldrobotSensorTeam/ldlidar_stl_ros)
```
rainer@jetsonautoware46:~/ldlidar_ros_ws$ 
roslaunch ldlidar_stl_ros ld06.launch
```
![](./media/ros-rviz.png)


## 3 python
```
git clone https://github.com/henjin0/LIDAR_LD06_python_loder.git
cd ~/projects/LIDAR_LD06_python_loder
python main.py 
```
or in this repo
```
cd ldrobot-D300-lidar-test
rainer@jetsonautoware46:~/projects/ldrobot-D300-lidar-test$ 
python ld06_main.py 
```

note: change port to correct value in *main.py*

![](./media/pythontest.png)

## [coordinate sytem / technical data](https://www.waveshare.com/wiki/DTOF_LIDAR_LD19)
LD19 uses the left-handed coordinate system, the front side of the sensor is defined as the x-axis (namely the zero direction), the rotation center is the coordinate origin, and the rotation angle increases along the clockwise direction. Please refer to the below photo:
![](media/DTOF-Coordinate.png)