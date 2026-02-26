---
title: ArcGIS Pro安装教程
date: 2026-01-01
tags:
  - ArcGISPro
  - GIS
draft: true
description: ArcGIS Pro安装教程
---
## ArcGIS Pro 3.3.2安装

>ArcGIS Pro 3.3.2安装教程
>https://malagis.com/arcgis-pro-3-3-2-learn-version-full-installation-tutorial.html


>下载地址
>
>链接: https://pan.baidu.com/s/1yLoQD9pwCSXXv3uURp5feA 提取码: mka9 解压密码：malagis.com


### 软件安装包清单拆解

- **1、windowsdesktop-runtime-8.0.4-win-x64.exe (环境配置)**
    
    - **作用**：这是微软的 .NET 运行库。ArcGIS Pro 3.x 是基于 .NET 开发的，没有它，软件连房子地基都打不稳，甚至打不开。
        
- **2、ArcGISPro_33_zh_CN_190105.exe (软件底座)**
    
    - **作用**：这是 **3.3 版本的核心基础包**。无论你想装 3.3.1 还是 3.3.2，都必须先运行这个文件。它负责把最核心的程序装进你的 `D:\software\ArcGISPro3.3.2` 文件夹里。
        
- **3、ArcGIS_Pro_332_190125.msp (升级补丁)**
    
    - **作用**：这是一个**升级包**。它不能独立运行，必须在安装完“文件 2”后运行。它会自动找到你装好的 3.3 软件，将其版本号从 3.3.0 提升到更稳定的 3.3.2。
        
- **4、ArcGISProHelp_33_zh_CN_19013...exe (中文帮助文档)**
    
    - **作用**：这是离线的**中文帮助包**。安装后，当你在软件里按 F1 或者查看工具说明时，显示的是中文而不是英文。
        
- **5、3.3.2PJ (激活补丁文件夹)**
    
    - **作用**：这是最关键的**“钥匙”**。里面通常包含 `AfCore.dll` 等文件。你需要手动把里面的文件复制到你 D 盘安装目录下的 `bin` 文件夹里，替换掉原文件，软件才能正常运行。





---


> [!summary] 安装教程合集
> 
>[ArcGIS Pro官方安装教程](https://pro.arcgis.com/zh-cn/pro-app/latest/get-started/install-and-sign-in-to-arcgis-pro.htm)
>[ArcGIS Pro 3.5 | 知乎](https://zhuanlan.zhihu.com/p/1934205529779077769)
>[ArcGIS 3.6安装 | 麻辣GIS](https://malagis.com/arcgis-pro-3-6-learn-version-full-installation-tutorial.html)



