# 上海电子信息职业技术学院-服务健康状态API原型


[GitHub IO主页](https://sonicdx.github.io/SHSP_STIEI_PrototypeDemo/)

[GitHub主页](https://github.com/sonicdx/SHSP_STIEI_PrototypeDemo/)

## 项目说明

​	通过 [**[Demo_Server_Launcher]**](https://github.com/sonicdx/SHSP_STIEI_PrototypeDemo/raw/master/Demo_Server_Launcher.7z) 与 [**[ServerMonitorDemo]**](https://github.com/sonicdx/SHSP_STIEI_PrototypeDemo/raw/master/ServerMonitorDemo.7z)  用来演示如何设计与验证符合 [STIEI-IDS-REF001[服务健康状态API规范]](https://sonicdx.github.io/STIEI_IDS_Documents/pages/STIEI-IDS-REF001.html) 的服务。

## 下载链接

+  [**[Demo_Server_Launcher]**](https://github.com/sonicdx/SHSP_STIEI_PrototypeDemo/raw/master/Demo_Server_Launcher.7z) 

  说明： SHSP服务端原型程序

+ [**[ServerMonitorDemo]**](https://github.com/sonicdx/SHSP_STIEI_PrototypeDemo/raw/master/ServerMonitorDemo.7z)

  说明：SHSP客户端原型程序

## 使用说明：

[Demo_Server_Launcher  详细说明](./Demo_Server_Launcher)

**运行 Demo_Server_Launcher.exe**

![Demo_Server_Launcher_ui](.\Images\Demo_Server_Launcher_ui.png)

​	**界面说明**

+ 服务连接： 服务的基本地址

+ 健康数据访问地址： 符合SHSP协议的API访问地址。使用鼠标点击可用浏览器直接查看API的返回结果。

+ 模拟MemorySize数值：可以修改SHSP API返回数据里的 `Summary:MemorySize` 的数值。该功能可用以测试与调试使用。

  ---

[ServerMonitorDemo  详细说明](./ServerMonitorDemo)

​	**程序界面**

![ServerMonitorDemo_ui](.\Images\ServerMonitorDemo_ui.png)

​	**界面说明**

+ 本地服务器

  + 轮训 **Demo_Server_Launcher** 程序模拟出SHSP服务器的状态。
  + 服务器状态： 如果查询 `本地服务器`的状态正确，显示为绿色的"在线"；否则为红色的"离线"。
  + 服务名称： 读取服务 SHSP 协议中的 *ServiceName* 项并显示。
  + 服务启动时间：读取服务 SHSP 协议中的 *start_utc* 项并以本地时间格式显示。该项下方显示服务器启动时间与现在的相对时间差。
  + 服务当前时间：读取服务 SHSP 协议中的 *time* 项并以本地时间格式显示。该项下方显示服务器启动时间与现在的相对时间差。
  + MemorySize：读取服务 SHSP 协议中的 *Summary:MemorySize* 项并显示。

+ 远程服务器

  基本同 *本地服务器*

+ 远程地址

  可以再设置一路其它符合SHSP协议的服务器地址（不带 */ShealthInfo* ），用以对比效果。
