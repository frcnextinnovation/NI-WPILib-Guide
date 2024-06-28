中文简体 | ...

# NI 环境搭建指南 (WPILib)

[![Next-Innovation](https://img.shields.io/badge/Next-Innovation-blueviolet?style=flat)](https://github.com/FRCNextInnovation) [![Lang](https://img.shields.io/badge/Lang-zh--CN-Green?style=flat)]() [![Lang](https://img.shields.io/badge/Ver-2024.7-blue?style=flat)]()

<img src="./assets/Logo_Purple_Word_Transparent.png" alt="Logo_Purple_Word_Transparent" style="zoom: 33%;" >

## WPILIB VSCode 安装指南

### 从 WPILib Docs 下载

1. 进入 **FRC 编程手册**官网

    [docs.wpilib.org](https://docs.wpilib.org/en/stable/index.html)

2. 进入 **WPILib Installation Guide**

    [WPILib Installation Guide](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html)

### 从 GitHub 下载

1. 进入 allwpilib GitHub 仓库

    [wpilibsuite/allwpilib](https://github.com/wpilibsuite/allwpilib)

2. 在 Releases 页面选择对应版本镜像下载

    [wpilibsuite/allwpilib/releases](https://github.com/wpilibsuite/allwpilib/releases)

### 安装

1. 右键管理员模式运行 Installer，点击 **Start **开始安装

    <img src="./assets/installer-start.png" alt="installer-start"/>

2. 点击 **Download VS Code for Single Install** (推荐)

    <img src="./assets/installer-vscode-download.png" alt="installer-vscode-download"/>

3. 选择 **Install for all User**，等待安装完成即可

    <img src="./assets/installer-options.png" alt="installer-options">

    <img src="./assets/installer-installing.png" alt="installer-installing">
    
    <img src="./assets/installer-finish.png" alt="installer-finish">

    > 注意: 你也可以选择在独立安装的 VSCode 插件市场上安装 WPILib 插件

5. 从桌面**快捷方式**启动 VSCode

    <img src="./assets/vscode.png" alt="vscode">


## 2. FRC其他重要程序的安装

1. **FRC Game Tools**

    包含: **LabVIEW Update**, **FRC Driver Station**, **FRC Utilities**(如 **roboRIO Imaging Tool**)

    [FRC Game Tools](https://download.ni.com/support/nipkg/products/ni-f/ni-frc-2024-game-tools/24.0/offline/ni-frc-2024-game-tools_24.0.2_offline.iso)

    - 选择 **I accept the above license agreement**，并继续

      <img src="./assets/ni-package-license.png" alt="ni-package-license">

    - 选择取消掉 Windows 的快速启动，并继续

      <img src="./assets/labview_fast_startup.png" alt="labview_fast_startup">

    - 选择继续，等待安装完成

      <img src="./assets/labview_package_manager_review.png" alt="labview_package_manager_review">

      <img src="./assets/ni-package-install.png" alt="ni-package-install">

      > 注意: 在这一步安装的过程中可能会出现报错，并自动跳到之前的安装界面，在这种情况下可以直接按照之前的选项继续安装，不用重新启动软件，这种情况一般是由于服务器连接不稳定造成的。

    - 如果看到这个页面，请继续选择安装，接下来的步骤与之前一致

      <img src="./assets/additional-software.png" alt="additional-software">

      <img src="./assets/labview_license_2.png" alt="labview_license_2">

      <img src="./assets/review-summary.png" alt="review-summary">

      <img src="./assets/detail-progress.png" alt="detail-progress">

    - 重启以完成安装

      <img src="./assets/installer-finish.png" alt="installer-finish">
      
      > 注意: 使用离线版安装器可以避免服务器连接不良导致的安装失败，离线版本的安装器可以在同链接下载。

2. **FRC Radio Configuration**

    用于：**配置机器人路由**

    [FRC Radio Configuration 24.0.1](https://firstfrc.blob.core.windows.net/frc2024/Radio/FRC_Radio_Configuration_24_0_1.zip)
    
3. **第三方**供应商

    用于：配置使用 CTRE 和 REV 等供应商产品

    [Phoenix Tuner X](https://github.com/CrossTheRoadElec/Phoenix-Releases/releases)

    - 在 CTRE Phoenix GitHub Releases 下载

    [REV Hardware Client](https://docs.revrobotics.com/rev-hardware-client)
    
    - 在 REV Docs 下载
    
      <img src="./assets/rev-hardware.png" alt="rev-hardware">
    
    - 安装后打开 **REV Hardware Client**
    
      <img src="./assets/rev.png" alt="rev">
    
    - 在 **Downloads** 界面下选择API下载即可(注意：2021年以后API将随REV客户端的安装自动安装)
    
      <img src="./assets/rev-hardware-downloads.png" alt="rev-hardware-downloads">
    


## 3. 检验环境

1. 进入**安装了 WPILib插件** 的 VSCode

2. 从右上角 **W 图标** 处启动插件。

3. 选择 "**新建一个项目**" (Create a new project)

4. 参照以下设置创建 Command Base 程序模板

    <img src="./assets/wpilib-main.png" alt="wpilib-main">

5. Build 程序(**一般会在第一次进入模板后自动执行**)，显示 **"Build Successful"** 即代表环境搭建完成，若出现 **"Build Failed"** 或 **其他字样** ，则是环境搭建**出现问题**，请参照之前步骤寻找原因

    <img src="./assets/build-robot-code.png" alt="build-robot-code">
