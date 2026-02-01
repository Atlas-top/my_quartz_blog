---
title: Quartz + Obsidian：打造属于自己的数字花园
date: 2026-02-01
tags:
  - Quartz
  - Obsidian
  - 数字花园
  - 静态网站
description: 介绍 Quartz 静态站点生成器、与 Obsidian 的结合，以及如何部署你的第一个博客。
draft: false
---

# 🌱 Quartz + Obsidian：打造自己的数字花园

在这个人人都能写作、人人都能发布的时代，**真正属于自己的空间**显得尤为重要。
我最终选择了 **Quartz + Obsidian** 的组合来搭建这座属于我的数字花园 —— 不依赖算法，不受平台限制，内容由自己掌控。

---

## 💡 什么是 Quartz？

**[Quartz](https://quartz.jzhao.xyz/)** 是一个开源的、功能全面的 **静态站点生成器（Static Site Generator）**，它可以把 Markdown 内容转换成具有漂亮布局和良好交互体验的网站。

* 📍 **官方网站**： [quartz.jzhao.xyz](https://quartz.jzhao.xyz/)
* 📦 **GitHub 项目**： [jackyzha0/quartz](https://github.com/jackyzha0/quartz)

⭐ **Quartz 项目价值与热度**：
该项目在 GitHub 上收获了 **11k+ ⭐ Star**，并拥有数千 Fork 与活跃使用者，是目前社区中备受欢迎的静态站点解决方案之一。

---

## ✨ Quartz 的核心优势

Quartz 与其它静态站点生成器相比，有几个非常突出的特点：

### 📌 1. 原生 Obsidian 支持
Quartz 从一开始就是为 Obsidian 生态设计的，它支持：
* **双链链接（Wikilinks）**：文章之间的 `[[链接]]` 可以直接跳转。
* **反向链接（Backlinks）**：自动显示“谁引用了这篇文章”。
* **图谱关系视图（Graph View）**：炫酷的交互式知识网络。
* **Callout 提示块**：Obsidian 里的漂亮提示框也能完美显示。

这些功能让你从 Obsidian 写出的笔记直接变成网站内容，保持丰富的关联性与网络结构。

### ⚡ 2. 极快性能 & 开箱即用
Quartz 默认集成了搜索、图谱、访客友好的布局等功能，而且构建速度非常快。

### 🎨 3. 高度可定制
无论是主题、样式还是页面结构，Quartz 都提供灵活的自定义能力，越高级的用户越能发掘其潜力。

---

## 🧠 Obsidian 简单介绍

在深入 Quartz 之前，先说一句：**我之后会写专门一篇文章介绍 Obsidian**，这里先简要说明它与 Quartz 结合的重要性。

**Obsidian** 是一款非常受欢迎的 Markdown 笔记软件，它最大的特点在于：

* 🗂 **本地优先**：笔记保存在本地 Markdown 文件中。
* 🔗 **双向链接**：让笔记之间形成网络化结构，而不是简单树状。
* 🧠 **知识管理思维**：“第二大脑”式的笔记方法。

这也正是 Quartz 最大的优势来源 —— Quartz 能最大程度 **保留 Obsidian 特性** 并在线呈现。

如果你还没用过 Obsidian，不用急，我会在后续文章详细讲解它如何提升写作与思考效率。

---

## 🛠️ Quartz 如何使用（以我的博客为例）

下面是我这次使用 Quartz 构建博客的大致流程。虽然官方提供了命令行方式，但我推荐使用更直观的 **"Docs as Code"** 工作流：

### ✅ 1. 初始化项目
（这一步通常只需要做一次，可以通过命令行完成，也可以直接 Fork 官方仓库）
```bash
git clone [https://github.com/jackyzha0/quartz.git](https://github.com/jackyzha0/quartz.git)
cd quartz
npm install
npx quartz create
```

### ✍️ 2. 日常写作 (Obsidian)

这是最舒服的部分：

- 打开 Obsidian，在 `content` 文件夹下新建笔记。

- 像平常一样写作，插入图片，使用双链。

- 所见即所得：你现在的笔记长什么样，网页上基本就长什么样。


### 🚀 3. 一键发布 (GitHub Desktop)

不需要敲复杂的代码，我使用 **GitHub Desktop** 来管理发布：

1. **Commit**：在软件左下角写个备注（比如“更新了新文章”），点击提交。

2. **Push**：点击右上角的 Push 按钮。

3. **自动上线**：GitHub 会自动通知云端服务器（Cloudflare Pages），大约 1 分钟后，你的网站就更新了！


> [!quote] 结语 如果你也想拥有一个长久、自由的数字空间，不妨试试这个组合。它门槛不高，但上限极高。

---

_本文发布于我的个人数字花园，转载请注明出处。_