---
title: Callout使用文档
date: 2026-01-10
draft: false
---
# Callout 使用指南（Obsidian / Quartz）

## 一、什么是 Callout？

**Callout（提示块）** 是一种用于“强调信息”的结构化内容块，常见于技术文档、知识库与数字花园中。

在 Obsidian 与 Quartz 中，Callout 本质上是 **带有语义的引用块（Blockquote）**，通过不同的类型（如 info、tip、warning）来表达：

- 这是在**解释概念**？
    
- 给读者一个**建议**？
    
- 提醒这里有**坑**？
    
- 还是引用一句**值得记住的话**？
    

合理使用 Callout，可以让文章：

- 📘 更像一份专业文档
    
- 🧠 信息层级更清晰
    
- 🌱 非常适合“数字花园 / 知识型博客”
    

---

## 二、Callout 的基础语法

所有 Callout 都遵循同一个基本结构：

```markdown
> [!类型] 标题（可选）
> 内容
```

要点说明：

- `>` 表示引用块（每一行都必须有）
    
- `[!类型]` 决定 Callout 的样式与语义
    
- **标题是可选的**，不写也可以
    

---

## 三、最常用的 Callout 类型（完整汇总）

下面所有示例，**均可直接复制到 Obsidian / Quartz 使用**。

---

### ℹ️ info —— 信息 / 说明（最常用）

用于：概念解释、背景说明、流程介绍

```markdown
> [!info] 技术说明
> 这是一套典型的 "Docs as Code"（像管理代码一样管理文档）的现代工作流。
```

> [!info] 技术说明
> 这是一套典型的 "Docs as Code"（像管理代码一样管理文档）的现代工作流。

---

### 💡 tip —— 技巧 / 建议

用于：经验总结、推荐做法

```markdown
> [!tip] 写作建议
> 建议在 Obsidian 中完成写作，再通过 Quartz 发布到网站。
```

> [!tip] 写作建议
> 建议在 Obsidian 中完成写作，再通过 Quartz 发布到网站。

---

### ✅ success —— 成功 / 正向结果

用于：完成提示、正反馈

```markdown
> [!success] 部署成功
> 当你看到这个页面，说明网站已经成功部署。
```

> [!success] 部署成功
> 当你看到这个页面，说明网站已经成功部署。

---

### ⚠️ warning —— 注意事项

用于：容易踩坑的地方

```markdown
> [!warning] 注意
> `content` 目录下如果没有 `index.md`，网站首页会直接 404。
```

> [!warning] 注意
> `content` 目录下如果没有 `index.md`，网站首页会直接 404。

---

### ❗ danger —— 高风险 / 严重警告

用于：可能导致严重问题的操作

```markdown
> [!danger] 高风险操作
> 不要在不了解 Git 的情况下强制推送到主分支。
```

> [!danger] 高风险操作
> 不要在不了解 Git 的情况下强制推送到主分支。

---

### 📝 note —— 备注 / 补充说明

用于：不影响主线，但值得一看的补充信息

```markdown
> [!note]
> Quartz 对 Obsidian 的 Callout 是原生支持的，无需额外插件。
```

> [!note]
> Quartz 对 Obsidian 的 Callout 是原生支持的，无需额外插件。

---

### ❓ question —— 提问 / 引导思考

用于：引导读者思考

```markdown
> [!question] 一个问题
> 如果没有平台推荐，你还会持续写作吗？
```

> [!question] 一个问题
> 如果没有平台推荐，你还会持续写作吗？

---

### 🔍 example —— 示例

用于：给出具体例子

```markdown
> [!example] 示例
> 例如：`[[Quartz]]` 可以直接链接到同名文章。
```

> [!example] 示例
> 例如：`[[Quartz]]` 可以直接链接到同名文章。

---

### 🧠 abstract / summary —— 总结

用于：段落或章节总结

```markdown
> [!summary] 本节小结
> Quartz 的优势在于：轻量、原生 Obsidian 支持、易部署。
```

> [!summary] 本节小结
> Quartz 的优势在于：轻量、原生 Obsidian 支持、易部署。

---

### 💬 quote —— 引用

用于：引用他人观点、格言

```markdown
> [!quote]
> 博客不是写给算法的，而是写给未来的自己。
```

> [!quote]
> 博客不是写给算法的，而是写给未来的自己。

---

## 四、无标题 Callout（更简洁）

如果你不需要标题，可以这样写：

```markdown
> [!info]
> 这是一个没有标题的 Callout。
```

> [!info]
> 这是一个没有标题的 Callout。

适合：

- 简短说明
    
- 插在段落中间
    

---

## 五、Callout 内使用强调样式（进阶）

### 1️⃣ 在 Callout 中使用加粗 / 代码

```markdown
> [!info]
> **Docs as Code** 强调：
> - 文档可版本控制
> - 可追溯、可协作
> - 与代码同等重要
```

> [!info]
> **Docs as Code** 强调：
> - 文档可版本控制
> - 可追溯、可协作
> - 与代码同等重要

---

### 2️⃣ 在 Callout 中使用蓝色强调文字

```markdown
> [!info] Docs as Code
> <span style="color:#3b82f6;">
> 这是一套典型的现代文档管理工作流。
> </span>
```

> [!info] Docs as Code
> <span style="color:#3b82f6;"> 这是一套典型的现代文档管理工作流。</span>

⚠️ 注意：Callout 内的 **每一行都要以 `>` 开头**。

---

## 六、写作建议：如何优雅地使用 Callout？

推荐使用原则：

- ✅ 一页不超过 3–5 个 Callout
    
- ✅ 用来“强调”，而不是承载全部内容
    
- ✅ 同一篇文章尽量统一使用几种类型
    

常见搭配示例：

- info + tip → 教程类文章
    
- warning + danger → 部署 / 运维文章
    
- quote + summary → 思考 / 随笔类文章
    

---

## 七、结语

Callout 不是装饰，而是一种 **结构化表达工具**。

当你开始有意识地使用它时，你的文章会自然从：

> “一大段文字”

进化为：

> “可阅读、可扫描、可长期维护的知识文档”。

这正是 Obsidian + Quartz 非常适合长期写作的原因之一 🌱