Installation
----



# Source
http://www.pyimagesearch.com/2017/03/27/how-to-install-dlib/


# Ubuntu 14.04 x64

Installing CMake, Boost, Boost.Python, and X11

```
sudo apt-get install build-essential cmake
sudo apt-get install libgtk-3-dev
sudo apt-get install libboost-all-dev
```
[1](http://www.pyimagesearch.com/2017/03/27/how-to-install-dlib/)



```
mkdir -p ~/dlib
cd ~/dlib
wget https://github.com/davisking/dlib/archive/v19.4.tar.gz
tar xf v19.4.tar.gz
rm v19.4.tar.gz
cd dlib-19.4/
```





# Testing dlib installation
```
cd examples
mkdir build && cd build
cmake ..
cmake --build . --config Release
```

[2](https://askubuntu.com/questions/824834/how-to-install-dlib-for-python3-in-ubuntu-14-04)
[3](http://dlib.net/compile.html)
[4](https://github.com/davisking/dlib)



doing a test

```
cd dlib/test
mkdir build && cd build
cmake ..
cmake --build . --config Release
./dtest --runall
```


# Installation


```
mkdir -p ~/dlib && cd ~/dlib && wget https://github.com/davisking/dlib/archive/v19.4.tar.gz && tar xf v19.4.tar.gz && rm v19.4.tar.gz
cd dlib-19.4/
mkdir build && cd build
cmake ..
sudo cmake --build . --target install
```
cmake --build . --config Release




```
git clone https://github.com/davisking/dlib
cd dlib
mkdir build
cmake ..
sudo cmake --build . --target install
```






```
.
.
.
-- Installing: /usr/local/include/dlib/image_keypoint/hessian_pyramid_abstract.h
-- Installing: /usr/local/include/dlib/image_keypoint/nearest_neighbor_feature_image_abstract.h
-- Installing: /usr/local/include/dlib/hash_set.h
-- Installing: /usr/local/include/dlib/entropy_decoder.h
-- Installing: /usr/local/include/dlib/hash_set
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_c.h
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_abstract.h
-- Installing: /usr/local/include/dlib/hash_set/hash_set_kernel_1.h
-- Installing: /usr/local/include/dlib/clustering.h
-- Installing: /usr/local/include/dlib/cpp_tokenizer.h
-- Installing: /usr/local/include/dlib/config.h
-- Installing: /usr/local/include/dlib/revision.h
-- Installing: /usr/local/share/doc/dlib/LICENSE.txt
-- Installing: /usr/local/lib/cmake/dlib/dlib.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlib-release.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlibConfig.cmake
-- Installing: /usr/local/lib/cmake/dlib/dlibConfigVersion.cmake
-- Installing: /usr/local/lib/pkgconfig/dlib-1.pc
map479-admin@eee320:~/dlib/dlib-19.4/build$
```



#  ./webcam_face_pose_ex


wget http://dlib.net/files/shape_predictor_68_face_landmarks.dat.bz2
bzip2 -d shape_predictor_68_face_landmarks.dat.bz2
./webcam_face_pose_ex











https://github.com/davisking/dlib/issues/395#issuecomment-271501699
