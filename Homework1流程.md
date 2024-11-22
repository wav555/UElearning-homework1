Homework1流程

主要参考链接

[(80 封私信 / 18 条消息) UE5安卓项目打包安装？ - 知乎](https://www.zhihu.com/question/573837498/answer/3212594550?utm_id=0&utm_source=wechat_session&utm_medium=social&s_r=0)

https://blog.csdn.net/ButDanJi/article/details/133919089?fromshare=blogdetail&sharetype=blogdetail&sharerId=133919089&sharerefer=PC&sharesource=m0_54935460&sharefrom=from_link

https://blog.csdn.net/qq_35587645/article/details/139207695?fromshare=blogdetail&sharetype=blogdetail&sharerId=139207695&sharerefer=PC&sharesource=m0_54935460&sharefrom=from_link

1.下载UE5.5

2.创建项目

![image-20241119205032562](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20241119205032562.png)

点击创建时出现报错如下

![image-20241119205200520](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20241119205200520.png)

可能是以下问题导致的

1. Win64平台被跳过

   - 输出中提到“Some Platforms were skipped due to invalid SDK setup: Win64.”，这意味着Win64平台的SDK设置不正确或缺失。这通常与Visual Studio或Windows SDK的安装有关。

2. 未找到有效的Visual C++工具链

   - 输出明确指出“No valid Visual C++ toolchain was found (minimum version 14.38.33130, preferred version 14.38.33130).”，这意味着您的系统上未安装满足要求的Visual C++工具链。

3. Visual Studio 2022安装要求

   - 输出建议安装Visual Studio 2022 17.8或更高版本，并确保选择了“MSVC v143 - VS 2022 C++ x64/x86 build tools (v14.38-17.8)”组件。

   重新创建了一个第一人称视角的项目，以上问题解决



下载并安装ADGE插件   翻墙才能下载

下载VS2022 

配置java环境

下载as

准备打包

[Android快速入门 | 虚幻引擎 4.27 文档 | Epic Developer Community | Epic Developer Community](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/android-quick-start?application_version=4.27)

https://blog.csdn.net/qq_35587645/article/details/139207695?fromshare=blogdetail&sharetype=blogdetail&sharerId=139207695&sharerefer=PC&sharesource=m0_54935460&sharefrom=from_link

配置android SDK

![image-20241120201930210](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20241120201930210.png)

在下载SDK时出现GPU报错问题

r.GpuProfilerMaxEventBufferSizeKB 256

打包失败

![image-20241121231329850](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20241121231329850.png)

尝试更改SDK版本\更改中英文\更改SDK路径都无法解决

遂放弃

打包windows

![image-20241122201222717](C:\Users\DELL\AppData\Roaming\Typora\typora-user-images\image-20241122201222717.png)