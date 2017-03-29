# SHSP客户端原型程序

[TOC]

## 基础环境

​	名称： ServerMonitorDemo

​	运行环境： .Net Framework 4.5.1

​	协议文档：[STIEI-IDS-REF001[服务健康状态API规范] ](https://sonicdx.github.io/STIEI_IDS_Documents/pages/STIEI-IDS-REF001.html)

## 使用说明

1. 运行 **ServerMonitorDemo.exe**

![ServerMonitorDemo_exe](.\Images\ServerMonitorDemo_exe.png)

2. 程序界面

![ServerMonitorDemo_ui](.\Images\ServerMonitorDemo_ui.png)

​	界面说明：

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

---

​	==操作方法：==

1. 修改远程地址 

   如果需要修改 *远程服务器地址* ，可在远程地址后的文本框内填写服务器访问地址（如：http://127.0.0.1:9091 ）。

   输入完后，需要点击 “Save” 按钮保存与起效。

