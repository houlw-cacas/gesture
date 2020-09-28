README
===========================
手势识别代码文档。

EVENT相机可视化工具jAER
----------

### How to run jAER
```Bash
unzip jaer-1.8.1.8.zip
```
```Bash
cd jaer-1.8.1.8
```
```Bash
chmod +x ./jAERViewer_linux.sh // if necessary
```
```Bash
./jAERViewer_linux.sh
```

### How to configure jAER
```Bash
AEChip->(select corresponding hardware)
```
```Bash
Interface->(select corresponding interface)
```
```Bash
File->remote->Enable unicast datagram(UDP) output->port:8991 bufferSize:8192
```
```Bash
View->Biases/HW Configuration->File->Load settings->(select an appropriate .xml file)
```
```Bash
View->Biases/HW Configuration->User-Friendly Controls->
Image Sensor : Capture Frames (on)
                Display Frames (off)
IMU: Enable (off) Display (off)
```

基于YOLO的手势识别工具
----------
### Requirements
* CMake>=3.12
* CUDA>=10.0	
* OpenCV>=2.4
* cuDNN>=7.0

### How to compile darknet on Linux
```Bash
unzip event_posture.zip
```
```Bash
cd event_posture/darknet
```
```Bash
cmake .
```
```Bash
make
```
### How to run darknet
```Bash
cd event_posture/darknet
```
```Bash
chmod +x ./run.sh
```
```Bash
./run.sh
```
