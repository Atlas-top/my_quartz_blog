---
title: RVC变声器
date: 2024-02-09
tags:
draft: false
description:
---
## Introduction

**RVC** ( Retrieval-based Voice Conversion-WebUI)，一个基于VITS的简单易用的变声框架。

>[!note]
>其通过“检索（Retrieval）”机制，从训练集中提取最接近的目标音色特征，从而显著提升变声的相似度和音质。相比早期的变声技术（如 So-VITS-SVC），RVC 对算力的要求更低，且转换速度更快。


该工具是由**B站大佬花儿不哭**发起的开源项目，目前已有 **34K+ Star** 🌟

![](</Attachments/image-22.webp>)


![](</Attachments/RVC变声器-20260207182142-1.webp>)


## Download&Install

### 1.RVC Github项目仓库下载

这里可以根据自己设备的显卡（N卡和A卡）选择对应的版本。

>[!warning]
>注意压缩包约有5.2个GB！
>提前预留好空间，保持网络连通！
>（我这里下载的是2.2.231006版本）

![](</Attachments/image-23.webp>)

### 2.B站（推荐）

小伙伴也可以直接去作者B站后台留言下载（并且，还可以学习和观看作者的官方教程）。


<div style="position: relative; width: 100%; height: 0; padding-bottom: 56.25%;">
    <iframe 
        src="https://player.bilibili.com/player.html?bvid=BV1pm4y1z7Gm&page=1&high_quality=1&as_wide=1&allowfullscreen=true" 
        style="position: absolute; width: 100%; height: 100%; left: 0; top: 0;" 
        scrolling="no" 
        border="0" 
        frameborder="no" 
        framespacing="0" 
        allowfullscreen="true"
        referrerpolicy="no-referrer"
    >
    </iframe>
</div>

### 3.解压和使用

#### 1️⃣下载好的压缩包，我们直接解压。

>[!Warning]
>注意解压路径不要出现中文字符！！！

#### 2️⃣使用前准备：下载模型

>[!info]
>这里我直接使用下载的模型来用于演示
>
>至于，**模型训练** 和**实时变声** 大家自行探索！

>模型下载：
>1.模型工坊
>https://mxgf.cc/
>
>2.妙音
>https://klrvc.com/
>
>3.Hugging Face | BanGDream 
>https://huggingface.co/Wanlau/RVC_BanGDream

这里我使用Hugging Face 上的一个原神（kazuha）角色做为演示。

【解压】

将下载的模型解压。例如这里我下载的是 kazuha-jp 100 epochs 48k v2.zip 
将会得到两个核心文件：`.pth` 模型文件 和 `.index` 特征索引文件

![](</Attachments/image-24.webp>)


>[!note]
>`.pth` 文件：复制并粘贴到 `RVC根目录\weights` 文件夹中。
`.index` 文件：放在`RVC根目录\RVC1006Nvidia\assets\weights` 中


【运行】

双击运行 `go-web.bat` 即可！

>[!warning]
>注意一些小伙伴由于一些原因可能会遇到报错（端口冲突）
>
>这时你可以试着将 `go-web.bat` 用记事本打开修改一下默认的 `7897` 端口！

![](</Attachments/image-25.webp>)


## Demonstration

RVC有两个界面一个是“训练推理界面”，一个是“实时变声界面”。

我们刚才运行的 `go-web.bat` 打开的就是 “训练推理界面” ，而运行 `go-realtime-gui.bat` 则打开的是 “实时变声界面” （没错，就是你平常听到的主播声音 😎）。

好了，这里我就以这个“训练推理界面” 进行一个简单的演示（至于如何实时变声，我想感兴趣的小伙伴们会自行探索），来看看效果！

![](</Attachments/image-21.webp>)


| 特性    | RVC WebUI (浏览器界面) | 实时变声 GUI (图中界面)     |
| ----- | ----------------- | ------------------- |
| 主要用途  | 模型训练、文件对文件转换、人声分离 | 直播、语音通话、实时游戏变声      |
| 模型通用性 | 训练出的模型（.pth）完全通用  | 使用 WebUI 训练好的模型进行推理 |
| 性能消耗  | 推理时消耗波动，适合高质量处理   | 极度优化延迟，追求响应速度       |
| 操作方式  | 通过浏览器点击，功能最全      | 独立窗口，专注参数调节         |

### 1.准备素材

>小编这里随别选了一首**李荣浩**的 **《年少有为》** 作为素材 ☺️

![](</Attachments/26.webp>)


### 2.素材处理

>将歌曲下载好之后，需要进行“伴奏人声分离”。这里我们可以直接使用RVC自带的伴奏分离功能

![](</Attachments/27.webp>)

### 3.下载Crayon Shin-chan声音模型

>HuggingFace
>https://huggingface.co/Roscall/shinchan/tree/main

### 4.开始转换（变声）

>在模型推理界面，我们需要设置一下参数：
>1.变调：设置为 12（即高一个八度）
>>由于男声的基频通常在 $100\text{--}150\text{ Hz}$，而童声或女声在 $200\text{--}300\text{ Hz}$ 左右，翻倍（+12）刚好能让声音进入目标角色的音域范围
>2.高音提取算法：rmvpe
>3.检索特征占比：0.7
>其它：暂时保持默认

### 5.成果展示

小编这里简单的做了个视频，一起来看看吧！






---
## 教程&资源


1. RVC GitHub项目仓库
https://github.com/RVC-Project/Retrieval-based-Voice-Conversion-WebUI

2. RVC作者官方使用教程  | B站 @花儿不哭
https://www.bilibili.com/video/BV1pm4y1z7Gm/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

3. 虚拟声卡下载（VB-Audio）
https://vb-audio.com/Cable/

4. RVC教程 | 知乎
https://zhuanlan.zhihu.com/p/670629290

5. RVC教程及安装包分享 | 知乎
https://zhuanlan.zhihu.com/p/1893425851233718834

6. RVC教程  | B站  | 模型训练（派大星）
https://www.bilibili.com/video/BV1NriRYcEqV/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

7. RVC教程 | B站  | 虚拟声卡使用
https://www.bilibili.com/video/BV1h52uBoEgb/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

8. RVC模型工坊
https://mxgf.cc/

9. RVC模型网站
https://klrvc.com/

10. Hugging Face模型  | 原神 / 米哈游系角色
https://huggingface.co/ArkanDash/rvc-genshin-impact/tree/main

11. Hugging Face | BanGDream 
https://huggingface.co/Wanlau/RVC_BanGDream

12. RVC安装教程 | B站  | 超详细保姆级 RVC变声器&虚拟声卡安装使用教程｜AI变声器｜开源AI变声器｜永久免费AI变声器
https://www.bilibili.com/video/BV189kBYzE9N/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

13. 虚拟声卡使用教程  | B站  |  voicemeeter下载安装使用
https://www.bilibili.com/video/BV1je5WzEEMy/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

14. Hugging Face space | RVC 项目官方模型库（**基础底模**和**系统组件**）
https://huggingface.co/lj1995/VoiceConversionWebUI/tree/main





