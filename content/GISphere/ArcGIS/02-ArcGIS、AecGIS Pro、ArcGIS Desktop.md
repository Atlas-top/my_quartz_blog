---
title: ArcGIS,AecGIS Pro,ArcGIS Desktop
date: 2025-02-07
tags:
  - ArcGIS
  - GIS
draft: false
description: ArcGIS、AecGIS Pro、ArcGIS Desktop概念辨析
---
### 1. 概念层级：从整体到具体

- **ArcGIS**：
    
    - **定义**：它是 Esri 公司推出的 **地理信息系统（GIS）产品家族的总称**。
    
    - **包含内容**：它不仅包含桌面端软件，还包含服务器端（ArcGIS Enterprise）、云端（ArcGIS Online）、移动端（各种 App）以及开发工具。
    
    - **比喻**：就像“Microsoft Office”是一个总称，包含了 Word、Excel 等。
    
- **ArcGIS Desktop**：
    
    - **定义**：它是 ArcGIS 家族中**传统的桌面端产品系列**。
    
    - **核心组件**：主要由 **ArcMap**（核心）、ArcCatalog、ArcScene 和 ArcGlobe 组成。
    
    - **现状**：它是基于 32 位架构的旧一代产品。目前 Esri 已经停止了它的新功能开发，正处于**维护和逐步淘汰阶段**。
    
- **ArcGIS Pro**：
    
    - **定义**：它是 Esri 推出的**下一代专业桌面 GIS 软件**。
    
    - **特点**：它是全新的 64 位架构，支持多线程处理，性能更强。它将 ArcMap 等多个软件的功能整合到了一个现代化的界面（类似 Office 的丝带状菜单）中。
    
    - **现状**：它是目前 Esri 的**旗舰级桌面产品**，也是未来的主流。
    

---

### 2. 核心区别对照表

| **特性**   | **ArcGIS Desktop (ArcMap)** | **ArcGIS Pro**                        |
| -------- | --------------------------- | ------------------------------------- |
| **软件架构** | 32 位（容易崩溃，利用硬件性能差）          | **64 位**（支持多线程，运行更快更稳）                |
| **界面风格** | 传统菜单和工具栏                    | **Ribbon 风格**（类似 Word/Excel，更现代）      |
| **数据展示** | 2D 和 3D 需在不同软件打开（Map/Scene） | **2D 和 3D 同步显示**（在一个项目里切换）            |
| **工程管理** | `.mxd`（一个文件一个地图）            | **`.aprx`**（一个项目可以包含多个地图和布局）          |
| **云端整合** | 弱，需要插件或繁琐操作                 | **强，深度集成** ArcGIS Online 和 Enterprise |
| **脚本支持** | Python 2.7                  | **Python 3.x**                        |


### 3. 三者的关系演变

1. **过去**：提到桌面 GIS，大家指的就是 **ArcGIS Desktop**（里面的 **ArcMap** 是大家最熟悉的软件）。

2. **现在**：Esri 正在推动用户从 ArcGIS Desktop **迁移**到 **ArcGIS Pro**。

3. **未来**：ArcGIS Desktop 会彻底退役，**ArcGIS Pro** 将成为 ArcGIS 家族中唯一的专业桌面端软件。
