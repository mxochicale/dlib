
# ROS-kinetic dependencies

install the following ROS-kinetic dependencies

```
sudo apt-get install ros-kinetic-roscpp ros-kinetic-tf ros-kinetic-std-msgs ros-kinetic-visualization-msgs ros-kinetic-sensor-msgs ros-kinetic-cv-bridge ros-kinetic-image-transport ros-kinetic-image-geometry
```



```
cd && git clone https://github.com/severin-lemaignan/gazr && cd gazr
mkdir build && cd build
```

modify at dlib/tools/show_head_pose.cpp
```
//if (waitKey(10) >= 0) break;
if (waitKey(10) == 27) break;
```

```
cmake -DWITH_ROS=ON -DDEBUG=OFF  -DCMAKE_BUILD_TYPE=Release ..
cmake -DWITH_ROS=ON -DDEBUG=ON  -DCMAKE_BUILD_TYPE=Release ..
```



```
make
```


testing gazr

```
./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
```






# Solved Issue
* [ ROS Kinetic dependencies are not working with gazr #12 ](https://github.com/severin-lemaignan/gazr/issues/12)
