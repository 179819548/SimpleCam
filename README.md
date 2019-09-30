<div align=center><img src="https://raw.githubusercontent.com/lmf12/SimpleCam/master/Images/image-head.jpg" width="450" height="150"/></div>

# 简介

本项目是基于 GPUImage 开源库构建的相机应用，主要用于学习交流目的。

# 界面预览

<div align=left><img src="https://raw.githubusercontent.com/lmf12/SimpleCam/master/Images/image-ui.jpg" width="600" height="355"/></div>

# 如何运行

本项目采用 CocoaPods 来引入第三方库，运行项目前，请先用终端进入项目根目录，执行 `pod install` 来下载第三方库。

在 v0.2.0 之后的版本，项目集成了 Face++ 人脸识别，需要你先去 Face++ 的官网申请 API Key，然后找到 `MGNetAccount.h` 文件，将申请好的 API Key 填入。整个申请过程比较简单，具体步骤可以参考 [这个文档](https://console.faceplusplus.com.cn/documents/5671787)。

当然，如果你懒得申请，本项目还提供了备选的人脸识别方案。备选方案通过 OpenCV + Stasm 的方式来实现。你可以在设置页中，自由切换使用的人脸识别引擎。只不过，备选方案的识别速度和准确度会大打折扣。

> **注意：** 由于 `OpenCV2-contrib` 这个库比较大，而且可能需要科学上网，如果你一时下载不成功，又急于运行本项目，可以考虑先体验 v0.1.0 的版本。

# 功能

* **拍照**
* **录制视频**（包括分段录制）
* **闪光灯**（包括关闭、打开、自动、常量 4 种类型）
* **画幅比例调节**（4 种比例）
* **前后置切换**
* **手动对焦**
* **焦距调整**
* **自定义抖音滤镜**  👉[效果预览](https://github.com/lmf12/SimpleCam/blob/master/Images/image-2.gif)
* **美颜滤镜**  👉[效果预览](https://github.com/lmf12/SimpleCam/blob/master/Images/image-1.gif)
* **人脸关键点识别**  👉[效果预览](https://github.com/lmf12/SimpleCam/blob/master/Images/image-3.gif)

# 相关文章

* [使用 GPUImage 实现一个简单相机](http://www.lymanli.com/2019/06/15/ios-gpuimage-camera/)
* [在 GPUImage 中检测人脸关键点](http://www.lymanli.com/2019/09/29/ios-gpuimage-face-detect/)

# 版本更新


| 版本号 | 更新日志 |
| --- | --- |
| v0.2.0 | 1. 集成 OpenCV + Stasm 人脸关键点识别 <br> 2. 集成 Face++ 人脸关键点识别 |
| v0.1.0 | 1. 完成一个基础相机框架搭建 <br> 2. 集成自定义抖音滤镜 <br> 3. 集成美颜滤镜 |

# 特别感谢

* [GPUImage](https://github.com/BradLarson/GPUImage)
* [Masonry](https://github.com/SnapKit/Masonry)
* [RSSwizzle](https://github.com/rabovik/RSSwizzle)
* [Toast](https://github.com/scalessec/Toast)
* [LFLiveKit](https://github.com/LaiFengiOS/LFLiveKit)
* [OpenCV](https://opencv.org/)
* [Stasm](http://www.milbo.users.sonic.net/stasm/)
* [Face++](https://www.faceplusplus.com.cn/)

# License

本项目采取 MIT 协议，具体条款请参见[这里](https://github.com/lmf12/SimpleCam/blob/master/LICENSE)。
