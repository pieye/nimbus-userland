<img src="./assets/PIEYE_Logo_RGB_POS.png" align="right"
     title="pieye logo" width="184" height="55">

# nimbus-userland
Raspberry pi embedded sources of nimbus

# installation
Follow these steps to install the latest stable version of nimbus userland
1. update to bleeding edge kernel (`sudo rpi-update`)
2. add nimbus apt repository
     - add line `deb http://apt.pieye.org/debian/ nimbus-stable main` to /etc/apt/sources.list
     - `wget -O - -q http://apt.pieye.org/apt.pieye.org.gpg.key | sudo apt-key add -`
     - `sudo apt-get update`
3. add line `dtoverlay=irs1125` to /boot/config.txt
4. `sudo apt-get install nimbus-server` or `sudo apt-get install libnimbus-dev`

# Authors
Markus Proeller

See also the list of contributors who participated in this project.

# License
This project is licensed under the GPLv3 License - see the LICENSE file for details

# 3rd party libraries
We use the following 3rd party libraries:
 
- JSON rpc server/client (MIT license), see https://github.com/cinemast/libjson-rpc-cpp
- catch2 (Boost Software License 1.0), see https://github.com/catchorg/Catch2
- libcurl, see https://curl.haxx.se/libcurl/ (copyright: https://curl.haxx.se/docs/copyright.html)
- libmicrohttpd (GNU LGPL v2.1), see https://www.gnu.org/software/libmicrohttpd/
- libjsoncpp, see https://github.com/open-source-parsers/jsoncpp (license: https://github.com/open-source-parsers/jsoncpp/blob/master/LICENSE)
- libargtable (GNU Library General Public License (LGPL)), see http://argtable.sourceforge.net/
- libhiredis (BSD 3-Clause "New" or "Revised" License), see https://github.com/redis/hiredis
- g3log (The Unlicense), see https://github.com/KjellKod/g3log
- gtest (BSD 3-Clause "New" or "Revised" License), see https://github.com/google/googletest
- openCL, see https://www.khronos.org/opencl/ (license: https://github.com/KhronosGroup/OpenCL-Headers/blob/master/LICENSE)
- simpleWebsocketServer (MIT license), see https://gitlab.com/eidheim/Simple-WebSocket-Server 
- ThreadPool (zlib license) https://github.com/progschj/ThreadPool
