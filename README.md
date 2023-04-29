# Realsense_jetson_for_jetpack_5
The realsense sdk and realsense-ros1 installation in jetson platform

1. Download the realsense sdk source (choose v2.50.0 for ros1): https://github.com/IntelRealSense/librealsense/archive/refs/tags/v2.50.0.zip
2. copy the install_jetson.sh to the librealsense-2.50.0
4. change the content of scripts/libuvc_installation.sh
```
#wget https://github.com/IntelRealSense/librealsense/archive/master.zip
#unzip ./master.zip -d .
#cd ./librealsense-master
cd /home/dji/Downloads/librealsense-2.50.0 # root of 2.50.0
```
3. install the sdk (only the Building from Source using RSUSB Backend can work for jetpack 5)
```
unzip librealsense-2.50.0
cd librealsense-2.50.0
sudo bash install_jetson.sh
```
