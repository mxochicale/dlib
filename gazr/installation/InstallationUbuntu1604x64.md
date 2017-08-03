#### Machine Features map479@map479-DQ57T

Webcam
```
$ lsusb
Bus 001 Device 005: ID 046d:0825 Logitech, Inc. Webcam C270
```

Machine
```
$ less /proc/cpuinfo
processor       : 0
vendor_id       : GenuineIntel
cpu family      : 6
model           : 30
model name      : Intel(R) Core(TM) i5 CPU         750  @ 2.67GHz
stepping        : 5
microcode       : 0x7
cpu MHz         : 1729.000
cache size      : 8192 KB
```

```
$ lshw -class memory
WARNING: you should run this program as super-user.
  *-memory                
       description: System memory
       physical id: 0
       size: 3883MiB
WARNING: output may be incomplete or inaccurate, you should run this program as super-user.

```


# Installation on 31 July 2017 @ map479@map479-DQ57T


### Python Dependencies for live_plot.py

```
sudo pip install numpy
sudo pip install matplotlib
```


gazr has been built with dlib https://github.com/davisking/dlib/archive/v19.4.tar.gz

```
cd && git clone https://github.com/severin-lemaignan/gazr && cd gazr
mkdir build && cd build
cmake -DWITH_ROS=OFF -DCMAKE_BUILD_TYPE=Release ..
```

in case of ros dependencies, you have to commend
```
//#include <ros/ros.h> at /src/head_pose_estimation.cpp
```

modify at /tools/show_head_pose.cpp
```
//if (waitKey(10) >= 0) break;
if (waitKey(10) == 27) break;
```


```
$ make
```


testing gazr

```
./gazr_show_head_pose --model ../share/shape_predictor_68_face_landmarks.dat  
```



```
./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```









# ISSUES


## usb2.0 plug

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





## live_plot.py


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

Install

```
sudo pip install numpy
sudo pip install matplotlib
```

and

```
 ./gazr_estimate_head_direction works well
```

```
./gazr_estimate_head_direction --model=../share/shape_predictor_68_face_landmarks.dat | python -u ../tools/live_plot.py
```
