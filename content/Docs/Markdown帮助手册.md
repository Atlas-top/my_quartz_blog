---
title: Markdown 写作完全指南（博客专业版）
date: 2026-02-02
tags:
  - Markdown
  - 写作规范
  - 博客搭建
  - Obsidian
description: 一份适合博客发布的 Markdown 完整教程，包含基础语法、进阶技巧、Callout 写作规范与实战示例。
updated: 2026-02-02
draft: false
---

# ✍️ Markdown 写作完全指南（博客专业版）

> [!quote] 为什么要学 Markdown？
> Markdown 不只是语法，而是一种 **结构化思维方式**。  
> 当你能用 Markdown 写清楚一篇文章，你已经学会了如何组织思想。

---

## 📚 本文你将学到什么？

- Markdown 的 **全部核心语法**
- 如何写出 **适合博客阅读** 的 Markdown
- Obsidian / Quartz 中的 **最佳实践**
- Callout 提示块的 **规范使用方式**
- 一套可以长期复用的 **写作模板**

---

## 🧭 目录

1. Markdown 是什么？
2. 标题与内容结构
3. 文本样式与强调
4. 列表的正确打开方式
5. 链接与图片
6. 代码块与技术写作
7. 引用与 Callout
8. 表格与任务列表
9. HTML 与样式扩展
10. 博客写作推荐规范
11. 完整示例模板

---

## 1️⃣ Markdown 是什么？

Markdown 是一种 **轻量级标记语言**，通过极少的符号完成结构表达：

- 易读
- 易写
- 易维护
- 天然适合版本控制（Git）

> [!info] 博客友好
> Markdown 是静态博客（如 Quartz、Hexo、Hugo）的事实标准。

---

## 2️⃣ 标题与内容结构（最重要）

### 标题语法


> [!tip] 写作建议
> 
> - 一篇博客 **只出现一个 `#`**
>     
> - 正文从 `##` 开始
>     
> - 不建议超过四级标题
>     

---

## 3️⃣ 文本样式与强调

### 基础强调

```markdown
**加粗**
*斜体*
***加粗 + 斜体***
~~删除线~~
```

效果示例：

**加粗**  
_斜体_  
_**加粗 + 斜体**_  
~~删除线~~

---

### 🎨 自定义颜色（Obsidian / Quartz 可用）

```markdown
<span style="color:#3b82f6">这是一段蓝色文字</span>
```

> [!warning] 注意  
> 不同平台对 HTML 支持程度不同，但 Quartz 完全支持。

---

## 4️⃣ 列表的正确打开方式

### 无序列表

```markdown
- Markdown
- Obsidian
- Quartz
```

### 有序列表

```markdown
1. 写作
2. 提交
3. 发布
```

### 嵌套列表（推荐）

```markdown
- 技术栈
  - Obsidian（写作）
  - Quartz（构建）
  - Cloudflare（部署）
```

---

## 5️⃣ 链接与图片

### 链接

```markdown
[Quartz 官网](https://quartz.jzhao.xyz/)
```

### 图片（博客常用）

```markdown
![图片说明](images/demo.png)
```

> [!tip] 图片建议
> 
> - 文件名使用英文
>     
> - 单独放在 `images / attachments` 目录
>     

---

## 6️⃣ 代码块与技术写作（核心）

### 行内代码

```markdown
使用 `git commit` 提交修改
```

### 多行代码块（推荐指定语言）

````markdown
```bash
git add .
git commit -m "update post"
git push
````

````

> [!info] 技术博客建议
> **所有代码都要进代码块**，不要直接写在正文里。

---

## 7️⃣ 引用与 Callout（重点）

### 普通引用

```markdown
> 这是一个普通引用
````

---

### Callout 提示块（Obsidian / Quartz）

#### ℹ️ info

```markdown
> [!info] 信息
> 用于背景说明、补充知识
```

#### 💡 tip

```markdown
> [!tip] 小技巧
> 给读者的实用建议
```

#### ⚠️ warning

```markdown
> [!warning] 注意
> 容易踩坑的地方
```

#### ❌ danger

```markdown
> [!danger] 高危操作
> 不建议新手尝试
```

#### ❓ question

```markdown
> [!question] 思考
> 抛出问题，引导读者
```

#### 📌 note（最常用）

```markdown
> [!note]
> 一段补充说明
```

---

## 8️⃣ 表格与任务列表

### 表格

```markdown
| 工具 | 用途 |
| ---- | ---- |
| Obsidian | 写作 |
| Quartz | 构建 |
| GitHub | 版本控制 |
```

### 任务列表

```markdown
- [x] 写作
- [x] 提交
- [ ] 发布
```

---

## 9️⃣ HTML 与样式扩展

Markdown 中可以直接使用 HTML：

```markdown
<div style="border-left:4px solid #3b82f6;padding-left:12px">
这是一个自定义强调块
</div>
```

> [!info]  
> Quartz 对 HTML 支持非常友好，适合进阶美化。

---

## 🔟 博客写作推荐规范（强烈建议）

> [!tip] 我的个人规范
> 
> - 一个章节一个主题
>     
> - 多用列表，少用大段文字
>     
> - 技术点一定配代码
>     
> - 解释用 Callout
>     

---

## 1️⃣1️⃣ 完整博客示例模板

````markdown
## 本文目标

> [!info]
> 本文将介绍 Quartz 的基本使用方式。

### 技术栈

- Obsidian
- Quartz
- GitHub
- Cloudflare Pages

### 操作步骤

```bash
git clone https://github.com/jackyzha0/quartz
````

> [!tip]  
> 新手建议先跑官方 demo。


---

## 🎯 结语

> [!quote]
> 写作不是为了展示技术，而是为了 **让未来的自己和别人看懂**。

Markdown 是工具，但真正重要的是：  
你是否在持续输出、持续思考、持续构建自己的知识体系。

---

*本文基于 Obsidian + Quartz 写作体系整理，可自由引用与修改。*
