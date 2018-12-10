OpenALPR with OpenCV 4 support

[![Build Status](https://travis-ci.org/sunfic/openalpr-opencv4.svg?branch=master)](https://travis-ci.org/sunfic/openalpr-opencv4)

Updated support for OpenCV 3.x and 4.x, dropped the support for OpenCV 2.x

Installation: 
-------
    sudo apt-get update
    sudo install -y libopencv-dev libtesseract-dev git cmake build-essential libleptonica-dev liblog4cplus-dev libcurl3-dev beanstalkd
    git clone https://github.com/sunfic/openalpr-opencv4
    cd openalpr-opencv4/src
    mkdir build
    cd build
    cmake ..
    make
    sudo make install


### Build with OpenCV 4:
1. For Ubuntu 18.04
   - Downgrade `libtesseract4` to `libtesseract3`
2. For Ubuntu 16.04 
   - update `liblog4cplus` compiled with C++11
   - pass `-std=c++11` to `CMAKE_CXX_FLAGS`
   
        ```cmake -DCMAKE_CXX_FLAGS=-std=c++11 ..```

License
-------

Affero GPLv3
http://www.gnu.org/licenses/agpl-3.0.html
