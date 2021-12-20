# YoloV4 Jetson Nano
![output image]( https://qengineering.eu/images/test_parkV4.jpg )
## YoloV4 with the ncnn framework. <br/>
[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)<br/><br/>
Paper: https://arxiv.org/pdf/2004.10934.pdf<br/><br/>
Special made for a Jetson Nano see [Q-engineering deep learning examples](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html)

------------

## Benchmark.
| Model  | size | objects | mAP | Jetson Nano 2015 MHz | RPi 4 64-OS 1950 MHz |
| ------------- | :-----:  | :-----:  | :-----:  | :-------------:  | :-------------: |
| [NanoDet](https://github.com/Qengineering/NanoDet-ncnn-Jetson-Nano) | 320x320 | 80 | 20.6  |  28.2 FPS | 13.0 FPS |
| [YoloV2](https://github.com/Qengineering/YoloV2-ncnn-Jetson-Nano) | 416x416  | 20 | 19.2 |  10.1 FPS | 3.0 FPS |
| [YoloV3](https://github.com/Qengineering/YoloV3-ncnn-Jetson-Nano) | 352x352 tiny | 20 | 16.6 | 17.7 FPS | 4.4 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Jetson-Nano) | 416x416 tiny | 80 | 21.7 | **11.2 FPS** | 3.4 FPS |
| [YoloV4](https://github.com/Qengineering/YoloV4-ncnn-Jetson-Nano) | 608x608 full | 80 | 45.3 | 0.7 FPS | 0.2 FPS |
| [YoloV5](https://github.com/Qengineering/YoloV5-ncnn-Jetson-Nano) | 640x640 small| 80 | 22.5 | 4.0 FPS | 1.6 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Jetson-Nano) | 416x416 nano | 80 | 25.8 | 17.6 FPS | 7.0 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Jetson-Nano) | 416x416 tiny | 80 | 32.8 | 8.3 FPS | 2.8 FPS |
| [YoloX](https://github.com/Qengineering/YoloX-ncnn-Jetson-Nano) | 640x640 small | 80 | 40.5 | 2.6 FPS | 0.9 FPS |

------------

## Dependencies.
### April 4 2021: Adapted for ncnn version 20210322 or later
To run the application, you have to:
- The Tencent ncnn framework installed. [Install ncnn](https://qengineering.eu/install-ncnn-on-jetson-nano.html) <br/>
- Code::Blocks installed. (`$ sudo apt-get install codeblocks`)

------------

## Installing the app.
To extract and run the network in Code::Blocks <br/>
$ mkdir *MyDir* <br/>
$ cd *MyDir* <br/>
$ wget https://github.com/Qengineering/YoloV4-ncnn-Jetson-Nano/archive/refs/heads/main.zip <br/>
$ unzip -j master.zip <br/>
Remove master.zip, LICENSE and README.md as they are no longer needed. <br/> 
$ rm master.zip <br/>
$ rm LICENSE <br/>
$ rm README.md <br/> <br/>
Your *MyDir* folder must now look like this: <br/> 
parking.jpg <br/>
busstop.jpg <br/>
YoloV4.cpb <br/>
yoloV4.cpp <br/>
yolov4-opt.param <br/><br/>
yolov4-tiny-opt.bin <br/>
yolov4-tiny-opt.param <br/><br/>

------------

## Running the app.
To run the application load the project file YoloV4.cbp in Code::Blocks.<br/> 
Next, follow the instructions at [Hands-On](https://qengineering.eu/deep-learning-examples-on-raspberry-32-64-os.html#HandsOn).<br/><br/>
You can switch between the YoloV4 tiny and the YoloV4 full version by the define at line 26<br/>
When deploying the full version, you have to download the 250 MB deep learning weight file yolov4-opt.bin from [Mega](https://mega.nz/file/Vsg02bJK#2h0QAd8ZUEykb6hi-yOcIAZKXnCBY0mevz8xkHYCmMM).<br/><br/>
Many thanks to [nihui](https://github.com/nihui/) again!<br/><br/>
![output image]( https://qengineering.eu/images/test_busV4.jpg )

------------

[![paypal](https://qengineering.eu/images/TipJarSmall4.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=CPZTM5BB3FCYL) 

