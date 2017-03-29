# SHSP服务端原型程序

[TOC]

## 基础环境

​	名称： Demo_Server_Launcher 

​	运行环境： .Net Framework 4.5.1

​	协议文档：[STIEI-IDS-REF001[服务健康状态API规范] ](https://sonicdx.github.io/STIEI_IDS_Documents/pages/STIEI-IDS-REF001.html)

## 使用说明

1. 运行 **Demo_Server_Launcher.exe**

![Demo_Server_Launcher_exe](.\Images\Demo_Server_Launcher_exe.png)

2. 程序界面

![Demo_Server_Launcher_ui](.\Images\Demo_Server_Launcher_ui.png)

​	界面说明：

+ 服务连接： 服务的基本地址
+ 健康数据访问地址： 符合SHSP协议的API访问地址。使用鼠标点击可用浏览器直接查看API的返回结果。
+ 模拟MemorySize数值：可以修改SHSP API返回数据里的 `Summary:MemorySize` 的数值。该功能可用以测试与调试使用。

3. 协议返回结果

![Demo_Server_Launcher_http_result](.\Images\Demo_Server_Launcher_http_result.png)