---
title: Quartz开启本地预览
date: 2026-01-22
tags:
  - Quartz
draft: true
description: 使用VScode修改Quartz代码，如和做到本地预览
---
## 1. 打开终端 (Terminal)


> [!warning] 注意
> 以管理员运行！！！


在 VS Code 里打开了你的 `my_quartz_blog` 文件夹。 如果底部没有终端窗口，按快捷键 **`Ctrl + ~`** (波浪号键) 或者点击顶部菜单栏 `Terminal -> New Terminal`

## 2. 输入“启动咒语”

在终端里输入下面这行命令，然后回车：

```Bash
npx quartz build --serve
```

>需要提提前安装 Node.js
>_(如果是第一次运行，它可能会问你是否安装 quartz，输入 `y` 回车即可)_
>https://nodejs.org/

## 3. 等待启动

终端会开始跑一堆代码，最后显示类似这样的一行绿色的字：

> **Quartz v4.x.x** **Started server at http://localhost:8080

## 4. 打开浏览器

按住 **Ctrl** 键，用鼠标点击终端里的那个链接 **`http://localhost:8080`**。 或者直接打开你的浏览器（Chrome/Edge），在地址栏输入 `localhost:8080`

## 5.如何停止？

当你改完想休息了，或者想去 Push 代码了：

1. 回到 VS Code 的终端。
    
2. 按 **`Ctrl + C`**。
    
3. 如果它问 `Terminate batch job (Y/N)?`，输入 `y` 回车。
    
4. 本地服务器就关闭了。


