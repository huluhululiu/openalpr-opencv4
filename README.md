OpenALPR with OpenCV 4 support

[![Build Status](https://travis-ci.org/sunfic/openalpr.svg?branch=master)](https://travis-ci.org/sunfic/openalpr)

Updated support for OpenCV 3.x and 4.x, dropped the support for OpenCV 2.x

Installation: 

git clone https://github.com/sunfic/openalpr
cd openalpr/src
mkdir build
cd build
cmake ..
make
sudo make install

If you encounter error "OpenCV 4.x+ requires enabled C++11 support", pass CMAKE_CXX_FLAGS to cmake
cmake -DCMAKE_CXX_FLAGS=-std=c++11 ..

Installation and usage please refer to: 
https://github.com/openalpr/openalpr

License
-------

Affero GPLv3
http://www.gnu.org/licenses/agpl-3.0.html
