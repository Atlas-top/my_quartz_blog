---
title: GKD
date: 2026-02-03
draft: false
updated: 2026-02-03
---
# GKD继李跳跳之后的另一款神器？！

Hello，小伙伴们！

时至今日，仍然有不少人，还在讨论「李跳跳」！！！

不由得有些感慨！于是就有了这篇文章！

真的很可惜，相信大家早已知道了「李跳跳」已于2023年8月，由于不可抗力的因素“无限期停止更新了”！😣作者这种纯粹的开发者精神，却在这个时代中无奈的“湮灭”了！

在前期，我也和大家简单说了说「李跳跳」这一款"生不逢时"的良心工具！虽然李跳跳这款神器在这个时代无奈退场，但却从未真正消失！

GKD这款免费开源的“基于无障碍 + 高级选择器 + 订阅规则的自定义屏幕点击应用”————不止于"跳广告"

接下来，我们就一起来看看这款神器吧！带你快速上手！

## 什么是GKD？

GKD或许可以说是「李跳跳」的“替代品”，但现在比「李跳跳」功能更加强大！

> 正如GitHub上的评价：GKD是"更加完美的李跳跳替代品"，但这个"完美"恰恰来自于它不止于替代的技术野心。

>GKD 是基于 **高级选择器 + 订阅规则 + 快照审查** 的自定义屏幕点击 Android 应用（An Android APP with custom screen tapping based on Accessibility, Advanced Selectors, and Subscription Rules）。通过自定义规则，在指定界面，满足指定条件(如屏幕上存在特定文字)时，点击特定的节点或位置或执行其他操作
>- 快捷操作。帮助你简化一些重复的流程, 如某些软件自动确认电脑登录
>- 跳过流程。某些软件可能在启动时存在一些烦人的流程, 这个软件可以帮助你点击跳过这个流程    (摘自gkd GItHub官方项目)

目前GKD，在GitHub上已有 **35.6K 个Star**🌟 **1.7K个 Fork** 🍴 可见其受欢迎的程度！


![](https://files.mdnice.com/user/55753/8a2737b2-696d-4576-8876-1170acde977f.png)


## GKD 下载安装

小伙伴们直接去GKD的官网：https://gkd.li/guide/
有详细的教程，这里我就不多介绍了。

## 订阅 导入规则

同「李跳跳」一样，如果你想跳过开屏广告，就需要自己手动写规则或导入大佬写好的规则，才可以正常使用。

这是第三方的大佬们写好的规则：https://github.com/topics/gkd-subscription


![](https://files.mdnice.com/user/55753/f9229953-1420-4643-9044-13a7310032aa.png)

## 开始使用

### 1.开启「无障碍权限」进行普通授权

同「李跳跳」一样，GKD需要基于Android 无障碍服务（Accessibility Service） 实现界面感知。**必须进行授权，否则GKD无法工作！**

#### ①点击这个小火箭🚀



![](https://files.mdnice.com/user/55753/49d83fdd-1522-4418-a2cd-8de6cf89f4ba.jpg)

进入授权模式选择“普通授权” → 进入到无障碍页面 → 在已下载应用里选择GKD开启即可


![](https://files.mdnice.com/user/55753/313d57a4-3573-45cf-b960-c60a107c8ba3.jpg)

#### ②进入“应用好电管理” 开其 “允许应用后台行为”


![](https://files.mdnice.com/user/55753/ac3f82fd-c37a-47f1-a2e6-eff5eae6349b.jpg)

这样即使你关机重启GKD任然在后台运行，不用再次重复授权！！！

### 2.高级授权（推荐）

> 推荐使用高级授权，使用Shizuku授权，可以 **降低功耗** 。GKD 功耗可降至约10mA级别，与 **「李跳跳」**相当！ 

高级授权有两种方式：
1.Shizuku 授权
2.adb 命令授权

由于本文只是带你简单快速上手，并且GKD的教程已经很多了（有兴趣的小伙伴们可以深入研究，GKD的功能远不止这些，本文再末尾也会提供一些大佬的教程），所以这里，我以Shizuku 授权进行简单演示。

#### ①下载Shizuku

在开始授权之前，我们需要下载　Shizuku。
关于下载地址：

https://shizuku.rikka.app/zh-hans/

也可以去酷安论会有大佬分享（记得给大佬投币支持一下）

#### ②启动Shizuku

在启动　Shizuku　之前，你需要打开“开发者选项”启用USB调试、无线调试，并进行配对。然后点击启动即可！



![](https://files.mdnice.com/user/55753/d0dedc9d-5859-42eb-aa35-0dd9edc0750a.jpg)

#### ③Shizuku授权

等等，暂停！正如上图所示，如果小伙伴们和我一样Shizuku出现了这样的警告，需要在“开发者模式”中关闭“权限监控”不同品牌和操作系统的设备解除限制的方法可以去看Shizuku的用户手册（包括一些详细教程）：`https://shizuku.rikka.app/zh-hans/guide/setup/#%E9%80%9A%E8%BF%87%E6%97%A0%E7%BA%BF%E8%B0%83%E8%AF%95%E5%90%AF%E5%8A%A8-%E9%80%9A%E8%BF%87%E8%BF%9E%E6%8E%A5%E7%94%B5%E8%84%91%E5%90%AF%E5%8A%A8-adb-%E6%9D%83%E9%99%90%E5%8F%97%E9%99%90`

好了，现在回到GKD授权，或着直接在Shizuku中直接进行GKD的授权即可！


![](https://files.mdnice.com/user/55753/dc65607c-6472-4f7b-868c-1bc38eeecfe4.jpg)



## 进阶玩法

前面说过 GKD 的功能不止跳广告，还可以实现 **自动化** 功能，例如：

- 自动签到

个平台的每日打卡，积分领取

- 自动确认

PC端微信登录却确认等等

- 以及自动抢红包等

- 自定义规则

如果第三方的订阅满足不了你的需求，你完全可以自己手写规则，实现更强大的功能。

> GKD 的教程目前已经非常多了，有很多大佬写的优秀教程！感兴趣的小伙伴可以去研究研究！本文在这里就不继续讨论了！☺️


## 参考资料以及资源整合

GKD官方网站等。及一些GKD的教程，以及高级玩法（编写自定义规则教程）

1. B站up主 @小in分享| GKD详细教程

https://www.bilibili.com/video/BV1BEc1eHE3F/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

2. B站 @小宇boi

https://www.bilibili.com/video/BV1VN411j7TR/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

3. B站 @差评君 | 李跳跳

https://www.bilibili.com/video/BV1Ym4y1T7ez/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

4. 李跳跳各个版本备份仓库

https://github.com/rongzhiy/LiTiaotiao?tab=readme-ov-file

5. 李跳跳自定义规则

https://snoopy1866.github.io/LiTiaotiao-Custom-Rules/

6.  GKD项目仓库

https://github.com/gkd-kit/gkd

7. GKD官方网站

https://gkd.li/
8. GKD第三方规则订阅

https://github.com/AIsouler/GKD_subscription

9. GKD规则编写教程

https://github.com/Snoopy1866/notebook/blob/main/04%20Others/GKD%20%E8%A7%84%E5%88%99%E7%BC%96%E5%86%99%E6%95%99%E7%A8%8B/gkd-rule-tutorial.md

10. B站up主 @epcdiy

https://www.bilibili.com/video/BV1zH4y1U7jG/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7

11. up主 @凇月落 | 手搓GKD自定义规则

https://www.bilibili.com/video/BV1BPVAzsETn/?share_source=copy_web&vd_source=4626b3a4121cb9f6a39cc37feb6ce0d7
