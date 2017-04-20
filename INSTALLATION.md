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

cd dlib-19.4/

cd examples
mkdir build
cd build
cmake ..
cmake --build . --config Release
```
[2](https://askubuntu.com/questions/824834/how-to-install-dlib-for-python3-in-ubuntu-14-04)
[3](http://dlib.net/compile.html)
[4](https://github.com/davisking/dlib)



## TEST 

```
cd dlib/test
mkdir build
cd build
cmake ..
cmake --build . --config Release
./dtest --runall
```






