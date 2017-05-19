Installation of gazr
----

(gazr)[https://github.com/severin-lemaignan/gazr/] is a library and a set of
tools for real-time gaze estimation from a monocular camera (typically, a webcam).


Requirements
This application requires dlib >= 18.18.


# On Ubuntu 14.04 x64

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



### ISSUES


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




#### Dependencies issues with dlibConfig.cmake when building gazr using dlib-19.4 in Release mode
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




### live_plot.py

```
sudo pip install numpy
sudo pip install matplotlib
```

```
$ ./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```






## Testing the camera configuration parameters
```
 ./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
Setting the optical center to (480, 360)
Processing time for this frame: 188.887ms
```
/show_head_pose.cpp
```
    // Configure the video capture
    // ===========================

        video_in.set(CV_CAP_PROP_FRAME_WIDTH, 640);
        video_in.set(CV_CAP_PROP_FRAME_HEIGHT, 480);
```

/estimate_head_direction.cpp
```
    // adjust for your webcam!
    estimator.focalLength = 500;

    // adjust for your webcam!
    video_in.set(CV_CAP_PROP_FRAME_WIDTH, 640);
    video_in.set(CV_CAP_PROP_FRAME_HEIGHT, 480);
    estimator.focalLength = 500;
    estimator.opticalCenterX = 80;
    estimator.opticalCenterY = 60;
```

/logitech-c920_640x360.ini
```
width
640
#960

height
360#720

```




# On Ubuntu 16.04 x64


gazr has been built with dlib https://github.com/davisking/dlib/archive/v19.4.tar.gz

```
cd && git clone https://github.com/severin-lemaignan/gazr && cd gazr && mkdir build && cd build
cmake -DCMAKE_BUILD_TYPE=Release ..
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
-- Found OpenCV: /usr/local (found version "3.2.0") found components:  core imgproc calib3d highgui
-- OpenCV version: 3.2.0
-- Found OpenCV: /usr/local (found version "3.2.0") found components:  core imgproc calib3d highgui imgcodecs videoio
-- Boost version: 1.58.0
-- Found the following Boost libraries:
--   program_options
-- Configuring done
-- Generating done
-- Build files have been written to: /home/map479/gazr/build
```

```
$ make
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


testing gazr

```
./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
```

I got an error for using usb2.0 plug

```
$ ./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
select timeout
select timeout
OpenCV Error: Assertion failed (total() == 0 || data != NULL) in Mat, file /home/map479/opencv-3.2.0/modules/core/include/opencv2/core/mat.inl.hpp, line 431
terminate called after throwing an instance of 'cv::Exception'
  what():  /home/map479/opencv-3.2.0/modules/core/include/opencv2/core/mat.inl.hpp:431: error: (-215) total() == 0 || data != NULL in function Mat

Aborted
```

Then I use a usb3.0 plug and I only got a view the webcam's window for a very short time.

```
$ ./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
Setting the optical center to (320, 240)
```







### live_plot.py


errors for python lib dependencies
```
$ ./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
/usr/local/lib/python2.7/site-packages/matplotlib/backend_bases.py:2453: MatplotlibDeprecationWarning: Using default event loop until function specific to this GUI is implemented
  warnings.warn(str, mplDeprecation)
invalid command name "140560397156176idle_draw"
    while executing
"140560397156176idle_draw"
    ("after" script)
Traceback (most recent call last):
  File "../tools/live_plot.py", line 41, in <module>
    plt.pause(0.05)
  File "/usr/local/lib/python2.7/site-packages/matplotlib/pyplot.py", line 300, in pause
    canvas.start_event_loop(interval)
  File "/usr/local/lib/python2.7/site-packages/matplotlib/backends/backend_tkagg.py", line 514, in start_event_loop
    FigureCanvasBase.start_event_loop_default(self,timeout)
  File "/usr/local/lib/python2.7/site-packages/matplotlib/backend_bases.py", line 2461, in start_event_loop_default
    self.flush_events()
  File "/usr/local/lib/python2.7/site-packages/matplotlib/backends/backend_tkagg.py", line 511, in flush_events
    self._master.update()
  File "/usr/local/lib/python2.7/lib-tk/Tkinter.py", line 1024, in update
    self.tk.call('update')
_tkinter.TclError: can't invoke "update" command: application has been destroyed


```

Then

```
sudo pip install numpy
sudo pip install matplotlib
```

and ./gazr_estimate_head_direction works well

```
./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```
