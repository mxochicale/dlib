Installation gazr which has a dlib dependency
----




# On Ubuntu 14.04 x64

Afer "sudo cmake --build . --target install"

```
cd
git clone https://github.com/severin-lemaignan/gazr && cd gazr && mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
make
```


to test the library.

```
./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
```


After cmake --build . --config Release

```
git clone https://github.com/severin-lemaignan/gazr && cd gazr && mkdir build && cd build
cmake -Ddlib_DIR=/home/map479-admin/dlib/dlib-19.4/build/dlib/config ..
make
```

References to install properly dlib and find  "~/dlib-19.4/build/dlib/config/dlibConfig.cmake"
https://github.com/davisking/dlib/issues/395#issuecomment-271501699
https://github.com/severin-lemaignan/gazr/issues/4#issuecomment-277940737
https://github.com/severin-lemaignan/gazr/issues/2#issuecomment-271183879

Brute force solution

```
CMake Error at /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:35 (include):
  include could not find load file:

    /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlib.cmake
Call Stack (most recent call first):
  CMakeLists.txt:11 (find_package)


CMake Error at /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:42 (include):
  include could not find load file:

    /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/use_cpp_11.cmake
Call Stack (most recent call first):
  CMakeLists.txt:11 (find_package)
```

```
$ sudo find ~/ -type f -name "dlib.cmake"
[sudo] password for map479-admin:
/home/map479-admin/dlib/dlib-19.4/build/dlib/CMakeFiles/Export/lib/cmake/dlib/dlib.cmake
$ sudo find ~/ -type f -name "use_cpp_11.cmake"
/home/map479-admin/dlib/dlib-19.4/dlib/cmake_utils/use_cpp_11.cmake
```
cd /home/map479-admin/dlib/dlib-19.4/build/dlib/config/
cp /home/map479-admin/dlib/dlib-19.4/build/dlib/CMakeFiles/Export/lib/cmake/dlib/dlib.cmake .

mkdir -p /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/
cd /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/
cp /home/map479-admin/dlib/dlib-19.4/dlib/cmake_utils/use_cpp_11.cmake .


then  more requirements

```
$ cmake ..
CMake Error at /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/use_cpp_11.cmake:19 (include):
  include could not find load file:

    /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/add_global_compiler_switch.cmake
Call Stack (most recent call first):
  /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:42 (include)
  CMakeLists.txt:11 (find_package)


-- C++11 activated.
CMake Error at /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/use_cpp_11.cmake:46 (add_global_compiler_switch):
  Unknown CMake command "add_global_compiler_switch".
Call Stack (most recent call first):
  /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:42 (include)
  CMakeLists.txt:11 (find_package)
```

so I go for "sudo cmake --build . --target install"


## FAILURE TRIALS
the reason was because
I only compile the examples instead of the main dlib project
```
cmake -Ddlib_DIR=-Ddlib_DIR=/home/map479-admin/dlib/dlib-19.4/dlib/ ..
cmake -Ddlib_DIR=-Ddlib_DIR=/home/map479-admin/dlib/dlib-19.4/dlib/cmake_utils ..
cmake -DCMAKE_BUILD_TYPE=Release ..
```

* where is ""-Ddlib_DIR=<dlib install path>/lib/cmake/dlib .. ?
Apparently is in this path
/dlib/dlib-19.4/dlib/cmake_utils/dlibConfig.cmake.in







# Testing




```
$ cmake ..
-- The C compiler identification is GNU 4.8.4
-- The CXX compiler identification is GNU 4.8.4
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- C++11 activated.
-- Found OpenCV: /usr/local (found version "3.2.0") found components:  core imgproc calib3d highgui
-- OpenCV version: 3.2.0
-- Found OpenCV: /usr/local (found version "3.2.0") found components:  core imgproc calib3d highgui imgcodecs videoio
-- Boost version: 1.54.0
-- Found the following Boost libraries:
--   program_options
-- Configuring done
-- Generating done
-- Build files have been written to: /home/map479-admin/mxochicale/github/gazr/build
```



# ISSUES


./gazr_show_head_pose ... is not working properly
https://github.com/severin-lemaignan/gazr/issues/8



gazr has been successfully built with dlib-19.4 on Ubuntu 14.04 x64 with OpenCV version: 3.2.0 and Boost version: 1.54. For building dlib-19.4, it has been used "sudo cmake --build . --target install"

Then, I try to test gazr as suggested
```
$ ./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
Setting the optical center to (320, 240)  
Processing time for this frame: 3464.05ms  
```
However, it only generates the previous two lines and I can also observe a quick
view of the window for a very short time.

I did another test with gazr_estimate_head_direction and live_plot.py with
```
$ ./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```
It seems to be working since the traces of Pitch Yaw Roll changed over time when
the webcam is pointing my face but the processing is very slowly.

I reckon, I am missing something to make it work. Do you have any comments?

P.S. "./webcam_face_pose_ex" in "~/dlib/dlib-19.4/examples/build" is working fine.

#### Machine Features

Webcam
```
$ lsusb
Bus 002 Device 010: ID 046d:0991 Logitech, Inc. QuickCam Pro for Notebooks
```

Machine
```
$ less /proc/cpuinfo
processor       : 0
vendor_id       : GenuineIntel
cpu family      : 6
model           : 37
model name      : Intel(R) Core(TM) i5 CPU         650  @ 3.20GHz
stepping        : 2
microcode       : 0xc
cpu MHz         : 1197.000
```
```
$ lshw -class memory
WARNING: you should run this program as super-user.
  *-memory                
       description: System memory
       physical id: 0
       size: 3751MiB
```


I appreciate your time and help.




NEXT 
https://wiki.archlinux.org/index.php/webcam_setup#Webcam_resolution




# Dependencies issues with dlibConfig.cmake when building gazr using dlib-19.4 in Release mode
https://github.com/severin-lemaignan/gazr/issues/9


I am trying to build dlib-19.4 in release mode to increase the processing
speed using "cmake --build . --config Release" but I have been facing the following dependencies
issues with dlibConfig.cmake:

```
$ cmake -Ddlib_DIR=/home/map479-admin/dlib/dlib-19.4/build/dlib/config ..
.
.
.
CMake Error at /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:35 (include):
  include could not find load file:

    /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlib.cmake
Call Stack (most recent call first):
  CMakeLists.txt:11 (find_package)


CMake Error at /home/map479-admin/dlib/dlib-19.4/build/dlib/config/dlibConfig.cmake:42 (include):
  include could not find load file:

    /home/map479-admin/dlib/dlib-19.4/include/dlib/cmake_utils/use_cpp_11.cmake
Call Stack (most recent call first):
  CMakeLists.txt:11 (find_package)
```

To solve the previous problem I installed  dlib-19.4 with
"sudo cmake --build . --target install" which is not the release mode.


However, I want to install both dlib and gazr in release mode.

Do you have any suggestions?




## live_plot.py

```
sudo pip install numpy
sudo pip install matplotlib
```

```
$ ./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```
