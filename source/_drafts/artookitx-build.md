---
title: artookitx-build
tags:
---
wsl linux中运行

cd :/mnt/d/wanganqing/Projects/Workspace-ar-test/artoolkitx/Source

./build.sh android
下载opencv2 解压到 Source\depends\android  include 和 lib 中
设置anroid sdk 环境变量 ，下载 linux sdk

安装cmake ，sudo apt update , sudo apt install cmake

wsl 改成 图形界面
https://learn.microsoft.com/zh-cn/windows/wsl/tutorials/gui-apps
安装 文件管理工具
安装好 edge ，就可以下载 android studio
打开 bin下的 studio.sh
设置代理  https://blog.csdn.net/yihui8/article/details/108186571
下载 33 sdk

export ANDROID_HOME=/home/waq/Android/Sdk
export JAVA_HOME=/mnt/d/wanganqing/Applications/java/graalvm-ee-java17-22.3.0-linux/
编辑vim .bashrc，放入环境变量
CMake Error: CMake was unable to find a build program corresponding to "Unix Makefiles".  CMAKE_MAKE_PROGRAM is not set.  You probably need to select a different build tool.
CMake Error: CMAKE_CXX_COMPILER not set, after EnableLanguage
CMake Error: CMAKE_C_COMPILER not set, after EnableLanguage
-- Configuring incomplete, errors occurred!

android studio sdk 中找到cmake ndk-bundle  安装
ln -snf ~/Android/Sdk/ndk/25.2.9519653 ~/Android/Sdk/ndk-bundle

重新执行完毕 ./build.sh android

就可以打开 \Source\ARXJ\ARXJProj 是 java项目
