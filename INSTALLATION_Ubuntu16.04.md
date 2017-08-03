
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


Installing CMake, Boost, Boost.Python, and X11

```
sudo apt-get install build-essential cmake
sudo apt-get install libgtk-3-dev
sudo apt-get install libboost-all-dev
```



```
cd
git clone https://github.com/davisking/dlib
cd dlib
mkdir build && cd build && cmake  -D WITH_JPEG=OFF  ..
sudo cmake --build . --target install
```

[More about --target install](https://github.com/davisking/dlib/issues/395#issuecomment-271501699)


#### testing

Comment the macros at dlib/examples/CMakeLists.txt LINE 150 such as #add_gui_example(3d_point_cloud_ex)
to avoid the compilation of other examples


```
cd ../examples/
mkdir build && cd build && cmake -D WITH_JPEG=OFF  ..
cmake --build .  --config Release
```


download the face landmarks
```
wget http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2
bzip2 -d shape_predictor_68_face_landmarks.dat.bz2
```

```
$ ./webcam_face_pose_ex
```


# WARNING
However,
after building dlib with "cmake  -D WITH_JPEG=OFF  .."
 the warning of "Corrupt JPEG data:" is still persists
 ```
 $ ./webcam_face_pose_ex
 Corrupt JPEG data: 4 extraneous bytes before marker 0xd7
 ```
