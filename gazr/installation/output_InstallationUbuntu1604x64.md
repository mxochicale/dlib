# Installation on 31 July 2017 @ map479@map479-DQ57T


```
$ cd && git clone https://github.com/severin-lemaignan/gazr && cd gazr && mkdir build && cd build
Cloning into 'gazr'...
remote: Counting objects: 385, done.
remote: Total 385 (delta 0), reused 0 (delta 0), pack-reused 385
Receiving objects: 100% (385/385), 69.38 MiB | 21.40 MiB/s, done.
Resolving deltas: 100% (228/228), done.
Checking connectivity... done.

```

```
$ cmake -DCMAKE_BUILD_TYPE=Release ..
-- The C compiler identification is GNU 5.4.0
-- The CXX compiler identification is GNU 5.4.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- C++11 activated.
-- Found OpenCV: /opt/ros/kinetic (found version "3.2.0") found components:  core imgproc calib3d highgui
-- OpenCV version: 3.2.0
-- Found OpenCV: /opt/ros/kinetic (found version "3.2.0") found components:  core imgproc calib3d highgui imgcodecs videoio
-- Boost version: 1.58.0
-- Found the following Boost libraries:
--   program_options
-- Configuring done
-- Generating done
-- Build files have been written to: /home/map479/gazr/build
```




```
$ make
make
Scanning dependencies of target gazr
[ 12%] Building CXX object CMakeFiles/gazr.dir/src/head_pose_estimation.cpp.o
[ 25%] Linking CXX shared library libgazr.so
[ 25%] Built target gazr
Scanning dependencies of target gazr_benchmark_head_pose_single_frame
[ 37%] Building CXX object CMakeFiles/gazr_benchmark_head_pose_single_frame.dir/tools/benchmark_head_pose_estimation_single_frame.cpp.o
[ 50%] Linking CXX executable gazr_benchmark_head_pose_single_frame
[ 50%] Built target gazr_benchmark_head_pose_single_frame
Scanning dependencies of target gazr_show_head_pose
[ 62%] Building CXX object CMakeFiles/gazr_show_head_pose.dir/tools/show_head_pose.cpp.o
[ 75%] Linking CXX executable gazr_show_head_pose
[ 75%] Built target gazr_show_head_pose
Scanning dependencies of target gazr_estimate_head_direction
[ 87%] Building CXX object CMakeFiles/gazr_estimate_head_direction.dir/tools/estimate_head_direction.cpp.o
[100%] Linking CXX executable gazr_estimate_head_direction
[100%] Built target gazr_estimate_head_direction
```
