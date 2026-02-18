---
title: 模组（Mod）
date:
tags:
  - Mincraft
draft: true
description:
---


## 什么是模组？

>模组（Modification 的缩写）是玩家或开发者创建的第三方内容，通过修改或扩展 Minecraft 的原始代码，为游戏添加新功能、新内容或改变原有机制。

---

| 维度       | 原版 Minecraft  | 模组修改后               |
| :------- | :------------ | :------------------ |
| **内容边界** | 官方设定的方块、物品、生物 | 无限扩展的新元素            |
| **玩法目标** | 生存 → 击败末影龙    | 工业化、魔法研究、太空探索等自定义目标 |
| **系统深度** | 基础合成、简单红石     | 复杂自动化、逻辑编程、物理模拟     |
| **视觉体验** | 默认材质、基础光影     | 高清材质、实时光追、自定义模型     |
| **游戏寿命** | 数十小时主线内容      | 数千小时的持续可玩性          |

---

原版 Minecraft 代码
    ↓
模组加载器（Forge/Fabric）注入"钩子"（Hook）
    ↓
模组代码通过钩子接入游戏核心
    ↓
运行时：原版代码 + 模组代码 = 修改后的游戏


>[!info]
>钩子（Hook）是程序设计中的一种技术，指在原有代码执行流程的特定位置"插入"自定义代码的机制，允许第三方在不修改原始源码的情况下改变或扩展程序行为。

>[!example]
>现实类比：快递包裹的"拦截点"
>├── 正常流程：发货 → 运输 → 签收
>├── 钩子点1：发货前检查（Hook before shipping）
>│   └── 插入：验货、打包加固
>├── 钩子点2：运输中中转（Hook during transit）
>│   └── 插入：改地址、加急处理
>└── 钩子点3：签收后（Hook after delivery）
>    └── 插入：安装服务、售后回访
>
>→ 原流程不变，但在关键点"钩入"额外操作


---

| 术语                     | 定义            | 与模组的关系               |
| :--------------------- | :------------ | :------------------- |
| **Mod**（模组）            | 修改游戏代码的第三方扩展  | 核心概念                 |
| **Plugin**（插件）         | 服务器端脚本，不改客户端  | 仅服务端，如 Bukkit/Spigot |
| **Data Pack**（数据包）     | 官方支持的 JSON 配置 | 轻量级"官方模组"            |
| **Resource Pack**（资源包） | 视觉/听觉资源替换     | 常与模组配合使用             |
| **Shader**（光影）         | GPU 渲染程序      | 模组的一种（渲染类）           |
| **Add-on**（基岩版附加）      | 基岩版官方模组格式     | 基岩版的"模组"             |
| **Behavior Pack**（行为包） | 基岩版修改游戏行为     | Add-on 的组成部分         |
| **Modpack**（整合包）       | 多个模组的预配置组合    | 模集的集合                |
| **Launcher**（启动器）      | 管理游戏版本和模组的工具  | 模组的运行平台              |


---

## 一、科技/工业类模组

| 模组名 | 加载器 | 核心玩法 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **IndustrialCraft 2 (IC2)** | Forge | 电力工业、机器自动化 | 欧盟电力网、核反应堆、量子装备 | 1.12.2为主 | ⭐⭐⭐ 工业鼻祖 |
| **BuildCraft** | Forge | 管道物流、自动化建筑 | MJ能量、采石场、蓝图系统 | 1.12.2 | ⭐⭐⭐ 物流开创 |
| **Thermal Expansion** | Forge | 热力机械、资源处理 | RF能量、红石通量、机器升级 | 1.12.2-1.20 | ⭐⭐⭐ 现代工业核心 |
| **Mekanism** | Forge | 高端科技、五倍矿处理 | 通用能量、核聚变、量子传送 | 1.12.2-1.20 | ⭐⭐⭐ 终极科技 |
| **Applied Energistics 2 (AE2)** | Forge | 存储网络、自动合成 | 频道系统、分子装配、空间塔 | 1.12.2-1.20 | ⭐⭐⭐ 物流终极方案 |
| **Create** | Forge/Fabric | 机械动力、物理仿真 | 齿轮传动、应力系统、动力机械 | 1.16.5-1.20 | ⭐⭐⭐ 近年最火 |
| **Immersive Engineering** | Forge | 复古工业、高压电 | 真实电线、大型机械、柴油发电机 | 1.12.2-1.20 | ⭐⭐⭐ 美学工业 |
| **Ender IO** | Forge | 末影科技、管道物流 | 物品/流体/能量管道、灵魂绑定 | 1.12.2 | ⭐⭐ 综合科技 |
| **Industrial Foregoing** | Forge | 工业先锋、农场自动化 | 激光钻、植物收获、动物牧养 | 1.12.2-1.20 | ⭐⭐ IC2精神续作 |
| **Refined Storage** | Forge | 简单存储网络 | 无线访问、自动合成（AE2简化版） | 1.12.2-1.20 | ⭐⭐ 入门存储 |
| **Extreme Reactors** | Forge | 大型核反应堆 | 多方块结构、蒸汽涡轮、钍燃料 | 1.12.2-1.20 | ⭐⭐ 能源方案 |
| **Draconic Evolution** | Forge | 龙系科技、顶级装备 | 能量核心、混沌守卫、飞行护盾 | 1.12.2-1.20 | ⭐⭐ 后期内容 |
| **Big Reactors** | Forge | 大型反应堆（Extreme前身） | 被动冷却、主动冷却 | 1.7.10-1.12.2 | ⭐⭐ 历史经典 |
| **NuclearCraft** | Forge | 核物理模拟 | 裂变/聚变、粒子加速器、辐射 | 1.12.2 | ⭐⭐ 硬核科学 |
| **Flux Networks** | Forge | 无线能量传输 | 跨维度能量、网络管理 | 1.12.2-1.20 | ⭐⭐ 能源辅助 |
| **Powah** | Forge | 新能源系统 | 反应堆、能量立方、充能台 | 1.16.5-1.20 | ⭐⭐ 轻量科技 |
| **Integrated Dynamics** | Forge | 逻辑编程、自动化控制 | 变量卡、逻辑运算、动态显示 | 1.12.2-1.20 | ⭐⭐ 编程向 |
| **RFTools** | Forge | 工具与维度 | 建造机、维度生成、屏幕系统 | 1.12.2-1.20 | ⭐⭐ 实用工具 |
| **ComputerCraft** | Forge | 电脑编程 | Lua脚本、海龟机器人、外设 | 1.12.2 | ⭐⭐ 编程教育 |
| **OpenComputers** | Forge | 高级电脑系统 | 组件化硬件、多语言支持、机器人 | 1.12.2 | ⭐⭐ 硬核编程 |

---

## 二、魔法/冒险类模组

| 模组名 | 加载器 | 核心玩法 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Thaumcraft 6** | Forge | 神秘时代、元素研究 | 魔导手册、注魔、邪术学 | 1.12.2 | ⭐⭐⭐ 魔法巅峰 |
| **Botania** | Forge/Fabric | 植物魔法、自然科技 | 花系统、魔力网络、无电力设计 | 1.12.2-1.20 | ⭐⭐⭐ 独特美学 |
| **Blood Magic** | Forge | 血魔法、恶魔仪式 | 生命源质、炼金术、召唤术 | 1.12.2-1.20 | ⭐⭐⭐ 黑暗魔法 |
| **Ars Nouveau** | Forge | 现代魔法、法术编程 | 魔符、仪式、魔源、自动化 | 1.16.5-1.20 | ⭐⭐⭐ 新兴热门 |
| **Astral Sorcery** | Forge | 星辉魔法、星座系统 | 大理石建筑、星能力、虹吸 | 1.12.2-1.20 | ⭐⭐⭐ 视觉震撼 |
| **Nature's Aura** | Forge | 自然灵气、生态平衡 | 灵气收集、仪式、森林保护 | 1.12.2-1.20 | ⭐⭐ 自然主题 |
| **Roots** | Forge | 德鲁伊魔法 | 仪式、草药、自然力量 | 1.12.2 | ⭐⭐ 经典魔法 |
| **Embers** | Forge | 余烬魔法、蒸汽朋克 | 余烬能量、炼金术、古代遗迹 | 1.12.2 | ⭐⭐ 复古风格 |
| **Mahou Tsukai** | Forge | 现代日式魔法 |  mana系统、法术卷轴、契约 | 1.16.5-1.20 | ⭐⭐ 动漫风格 |
| **Iron's Spells 'n Spellbooks** | Forge | RPG法术系统 | 法术书、施法、职业系统 | 1.18-1.20 | ⭐⭐ 动作魔法 |
| **Twilight Forest** | Forge | 暮色森林维度 | 迷宫、Boss战、进度解锁 | 1.12.2-1.20 | ⭐⭐⭐ 经典维度 |
| **The Aether** | Forge/Fabric | 天境维度、浮空岛 | 青铜/白银/黄金地牢 | 1.12.2-1.20 | ⭐⭐⭐ 最早维度 |
| **Blue Skies** | Forge | 蔚蓝浩空双维度 | Everbright/Everdawn、新生态 | 1.16.5-1.20 | ⭐⭐ 高完成度 |
| **The Undergarden** | Forge | 地下花园维度 | 乌特兰生态、独特矿石 | 1.16.5-1.20 | ⭐⭐ 地下探索 |
| **Alex's Mobs** | Forge | 丰富新生物 | 80+真实生态行为动物 | 1.16.5-1.20 | ⭐⭐⭐ 生物第一 |
| **Lycanites Mobs** | Forge | 恐怖怪物、事件系统 | 元素生物、随机事件、恐惧 | 1.12.2-1.20 | ⭐⭐ 硬核生存 |
| **Ice and Fire** | Forge | 龙与地下城 | 龙、独眼巨人、塞壬、神话生物 | 1.12.2-1.20 | ⭐⭐⭐ 冒险必装 |
| **Mowzie's Mobs** | Forge | 精致Boss生物 |  Ferrous Wroughtnaut、Barako | 1.12.2-1.20 | ⭐⭐ 战斗设计 |
| **The Betweenlands** | Forge | 交错维度、沼泽生态 | 腐烂机制、独特工具、Boss | 1.12.2 | ⭐⭐ 硬核维度 |
| **Atum 2** | Forge | 埃及沙漠维度 | 法老、金字塔、新制作系统 | 1.12.2-1.20 | ⭐⭐ 文化主题 |

---

## 三、优化/辅助类模组（必备基础）

| 模组名 | 加载器 | 核心功能 | 性能提升 | 版本支持 | 必备度 |
|:---|:---|:---|:---:|:---|:---:|
| **Sodium** | Fabric | 现代渲染引擎重写 | 2-10倍帧数 | 1.16.5-1.20 | ⭐⭐⭐ Fabric必装 |
| **Iris** | Fabric | 光影加载器 | 兼容Sodium | 1.16.5-1.20 | ⭐⭐⭐ 光影必备 |
| **Lithium** | Fabric | 游戏逻辑优化 | 减少卡顿 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Phosphor** | Fabric | 光照引擎优化 | 区块加载加速 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Indium** | Fabric | Sodium与Fabric兼容层 | 稳定性 | 1.16.5-1.20 | ⭐⭐ |
| **Embeddium** | Forge | Sodium的Forge移植 | 2-10倍帧数 | 1.20.1+ | ⭐⭐⭐ Forge新选择 |
| **OptiFine** | Forge/独立 | 光影/性能/动态光源 | 中等 | 全版本 | ⭐⭐ 逐渐被替代 |
| **FerriteCore** | Forge/Fabric | 内存占用压缩 | 减少50%+内存 | 1.16.5-1.20 | ⭐⭐⭐ 低内存必装 |
| **ModernFix** | Forge/Fabric | 启动速度优化 | 启动快数倍 | 1.16.5-1.20 | ⭐⭐⭐ |
| **LazyDFU** | Fabric | 数据修复优化 | 启动加速 | 1.16.5-1.20 | ⭐⭐ |
| **Starlight** | Fabric | 光照引擎重写 | 区块生成加速 | 1.16.5-1.20 | ⭐⭐⭐ |
| **JEI (Just Enough Items)** | Forge/Fabric | 配方查看/物品管理 | - | 1.12.2-1.20 | ⭐⭐⭐ 合成必备 |
| **REI (Roughly Enough Items)** | Fabric | JEI的Fabric替代品 | - | 1.16.5-1.20 | ⭐⭐⭐ |
| **EMI (Enough Items)** | Forge/Fabric | JEI现代替代品 | 更快更轻 | 1.19-1.20 | ⭐⭐ 新兴 |
| **Jade** | Forge/Fabric | 方块信息显示（Waila续作） | - | 1.16.5-1.20 | ⭐⭐⭐ |
| **The One Probe (TOP)** | Forge | 信息面板显示 | - | 1.12.2-1.20 | ⭐⭐ |
| **AppleSkin** | Forge/Fabric | 饥饿值/饱和度可视化 | - | 1.12.2-1.20 | ⭐⭐⭐ |
| **JourneyMap** | Forge/Fabric | 小地图/路径点/死亡标记 | - | 1.12.2-1.20 | ⭐⭐⭐ 导航必备 |
| **Xaero's Minimap** | Forge/Fabric | 轻量小地图 | - | 1.12.2-1.20 | ⭐⭐⭐ |
| **Xaero's World Map** | Forge/Fabric | 全屏世界地图 | - | 1.12.2-1.20 | ⭐⭐⭐ |
| **Controlling** | Forge/Fabric | 按键冲突管理 | - | 1.12.2-1.20 | ⭐⭐⭐ |
| **Inventory Profiles Next** | Fabric | 一键整理/自动补货 | - | 1.16.5-1.20 | ⭐⭐⭐ |
| **Inventory Tweaks Renewed** | Forge | 背包整理 | - | 1.12.2-1.20 | ⭐⭐ |
| **Mouse Tweaks** | Forge/Fabric | 鼠标拖拽优化 | - | 1.12.2-1.20 | ⭐⭐⭐ |
| **Item Scroller** | Fabric | 快速物品移动 | - | 1.16.5-1.20 | ⭐⭐ |
| **ShulkerBoxTooltip** | Fabric | 潜影盒内容预览 | - | 1.16.5-1.20 | ⭐⭐ |
| **Mod Menu** | Fabric | 模组列表管理 | - | 1.16.5-1.20 | ⭐⭐⭐ Fabric必装 |
| **Catalogue** | Forge | 模组菜单（Mod Menu替代品） | - | 1.18-1.20 | ⭐⭐ |
| **Configured** | Forge/Fabric | 游戏内配置编辑 | - | 1.16.5-1.20 | ⭐⭐⭐ |
| **Cloth Config** | Forge/Fabric | 配置界面API | - | 1.16.5-1.20 | ⭐⭐⭐ 依赖库 |
| **Bad Wither No Cookie** | Forge/Fabric | 禁用凋零音效 | - | 1.12.2-1.20 | ⭐⭐ |
| **Light Overlay** | Forge/Fabric | 亮度等级显示 | - | 1.12.2-1.20 | ⭐⭐⭐ 刷怪塔必备 |
| **MiniHUD** | Fabric | 信息HUD显示 | - | 1.16.5-1.20 | ⭐⭐ 技术玩家 |
| **Tweakeroo** | Fabric | 生存辅助工具集 | - | 1.16.5-1.20 | ⭐⭐ 技术玩家 |
| **Litematica** | Fabric | 投影模组/建筑辅助 | - | 1.16.5-1.20 | ⭐⭐⭐ 建筑必备 |
| **ItemSwapper** | Fabric | 快速物品切换 | - | 1.19-1.20 | ⭐⭐ |

---

## 四、建筑/装饰类模组

| 模组名 | 加载器 | 核心内容 | 特色功能 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Chisel** | Forge | 凿子装饰方块 | 数百种材质变体 | 1.12.2 | ⭐⭐⭐ 建筑经典 |
| **Chipped** | Forge/Fabric | Chisel现代版 | 更多材质、更好兼容 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Macaw's Doors** | Forge/Fabric | 多样门设计 | 数十种风格门 | 1.12.2-1.20 | ⭐⭐⭐ 建筑细节 |
| **Macaw's Windows** | Forge/Fabric | 多样窗户设计 | 百叶窗、拱形窗等 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Macaw's Roofs** | Forge/Fabric | 屋顶方块 | 多种角度、材质 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Macaw's Bridges** | Forge/Fabric | 桥梁结构 | 绳索桥、木桥等 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Macaw's Trapdoors** | Forge/Fabric | 活板门变体 | 多样设计 | 1.16.5-1.20 | ⭐⭐ |
| **Macaw's Lights** | Forge/Fabric | 灯具设计 | 路灯、吊灯、壁灯 | 1.16.5-1.20 | ⭐⭐ |
| **MrCrayfish's Furniture Mod** | Forge | 现代家具 | 沙发、电视、冰箱等功能家具 | 1.12.2-1.20 | ⭐⭐⭐ 经典家具 |
| **Handcrafted** | Forge/Fabric | 精致家具 | 陶艺、织物、雕刻 | 1.18-1.20 | ⭐⭐ 新兴热门 |
| **Farmers Delight** | Forge/Fabric | 田园厨具 | 烹饪系统、田园美学 | 1.16.5-1.20 | ⭐⭐⭐ 生活+建筑 |
| **Supplementaries** | Forge/Fabric | 实用小物件 | 笼子、风向标、沙漏、烛台 | 1.16.5-1.20 | ⭐⭐⭐ 细节丰富 |
| **Decorative Blocks** | Forge/Fabric | 装饰方块 | 篝火、座椅、横梁 | 1.16.5-1.20 | ⭐⭐ |
| **Architect's Palette** | Forge/Fabric | 建筑师调色板 | 新方块、新材质 | 1.16.5-1.20 | ⭐⭐ |
| **BlockCarpentry** | Forge | 可变形方块 | 自定义外观、多种形状 | 1.16.5-1.20 | ⭐⭐ |
| **FramedBlocks** | Forge | 框架方块 | 任意材质贴图 | 1.16.5-1.20 | ⭐⭐ |
| **Rechiseled** | Forge/Fabric | 凿子替代品 | 连接材质、多样变体 | 1.18-1.20 | ⭐⭐ |
| **Every Compat** | Forge/Fabric | 模组兼容 wood types | 自动为其他模组生成家具 | 1.18-1.20 | ⭐⭐ 兼容性 |
| **Another Furniture** | Forge/Fabric | 额外家具 | 椅子、桌子、架子 | 1.18-1.20 | ⭐⭐ |
| **Dramatic Doors** | Forge/Fabric | 高门/双开门 | 3格高门、动画门 | 1.18-1.20 | ⭐⭐ |
| **Glassential** | Forge/Fabric | 功能性玻璃 | 幽灵玻璃、发光玻璃等 | 1.12.2-1.20 | ⭐⭐ |

---

## 五、农业/生活类模组

| 模组名 | 加载器 | 核心内容 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Pam's HarvestCraft 2** | Forge | 农业扩展 | 数十种作物、数百种食物 | 1.16.5-1.20 | ⭐⭐⭐ 农业之王 |
| **Croptopia** | Forge/Fabric | HarvestCraft现代替代 | 更多作物、简单配置 | 1.16.5-1.20 | ⭐⭐⭐ 轻量农业 |
| **Farmer's Delight** | Forge/Fabric | 田园烹饪 | 烹饪锅、切菜板、堆肥 | 1.16.5-1.20 | ⭐⭐⭐ 生活化 |
| **Serene Seasons** | Forge | 季节变化 | 温度、作物生长周期 | 1.12.2-1.20 | ⭐⭐⭐ 真实感 |
| **Tough As Nails** | Forge | 生存难度提升 | 体温、口渴、疾病 | 1.12.2-1.20 | ⭐⭐ 硬核生存 |
| **Simple Farming** | Forge/Fabric | 简单农业 | 新作物、果树、酿造 | 1.16.5-1.20 | ⭐⭐ |
| **Berry Good** | Forge | 浆果扩展 | 更多浆果种类 | 1.16.5-1.20 | ⭐⭐ |
| **Autumnity** | Forge | 秋季生态 | 枫树、蜗牛、新生物群系 | 1.16.5-1.20 | ⭐⭐ 季节主题 |
| **Neapolitan** | Forge | 冰淇淋主题 | 香草/巧克力/草莓系统 | 1.16.5-1.20 | ⭐⭐ 美食向 |
| **Respite** | Forge | 茶饮系统 | 多种茶叶、效果 | 1.18-1.20 | ⭐⭐ |
| **Brewin' And Chewin'** | Forge | 酿造与发酵 | 酒精、奶酪、发酵 | 1.18-1.20 | ⭐⭐ |
| **Miner's Delight** | Forge | 矿工食物 | 洞穴烹饪、便携食物 | 1.18-1.20 | ⭐⭐ |
| **Ecologics** | Forge/Fabric | 生态改进 | 新树木、椰子、企鹅 | 1.18-1.20 | ⭐⭐ |
| **Storage Drawers** | Forge | 抽屉存储 | 量化显示、抽屉控制器 | 1.12.2-1.20 | ⭐⭐⭐ 存储经典 |
| **Framed Compacting Drawers** | Forge | 压缩抽屉 | 自动压缩存储 | 1.16.5-1.20 | ⭐⭐ |
| **Comforts** | Forge/Fabric | 睡眠辅助 | 睡袋、吊床 | 1.12.2-1.20 | ⭐⭐ |
| **Waystones** | Forge/Fabric | 传送石碑 | 命名传送、经验消耗 | 1.12.2-1.20 | ⭐⭐⭐ 探索必备 |
| **GraveStone Mod** | Forge/Fabric | 死亡墓碑 | 物品保护、定位 | 1.12.2-1.20 | ⭐⭐⭐ 防掉落 |
| **Corpse** | Forge/Fabric | 尸体系统 | 死亡尸体、物品保护 | 1.16.5-1.20 | ⭐⭐ GraveStone替代 |
| **Traveler's Backpack** | Forge/Fabric | 旅行者背包 | 大容量、工具槽、睡袋 | 1.16.5-1.20 | ⭐⭐⭐ 探索必备 |
| **Sophisticated Backpacks** | Forge | 高级背包 | 升级系统、自动化 | 1.16.5-1.20 | ⭐⭐⭐ 功能丰富 |

---

## 六、生物/生态类模组

| 模组名 | 加载器 | 核心内容 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Alex's Mobs** | Forge | 真实生态动物 | 80+动物、独特行为、掉落物 | 1.16.5-1.20 | ⭐⭐⭐ 生物第一 |
| **Lycanites Mobs** | Forge | 恐怖元素生物 | 事件系统、元素分类、恐惧 | 1.12.2-1.20 | ⭐⭐ 硬核生存 |
| **Ice and Fire** | Forge | 神话生物 | 龙、独眼巨人、海妖、鸡蛇 | 1.12.2-1.20 | ⭐⭐⭐ 冒险必装 |
| **Mowzie's Mobs** | Forge | 精致Boss | Ferrous Wroughtnaut、Barako | 1.12.2-1.20 | ⭐⭐ 战斗设计 |
| **BetterEnd** | Fabric | 末地生态大修 | 新生物群系、植物、材料 | 1.16.5-1.20 | ⭐⭐⭐ 地形神作 |
| **BetterNether** | Fabric | 下界生态大修 | 新森林、洞穴、材料 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Oh The Biomes You'll Go (BYG)** | Forge/Fabric | 生物群系扩展 | 80+新群系 | 1.16.5-1.20 | ⭐⭐⭐ 群系之王 |
| **Biomes O' Plenty** | Forge | 经典群系模组 | 多样生态、子群系 | 1.12.2-1.20 | ⭐⭐⭐ 老牌经典 |
| **Terralith** | Forge/Fabric | 地形生成器 | 全新地形、洞穴、结构 | 1.18-1.20 | ⭐⭐⭐ 地形神作 |
| **William Wythers' Overhauled Overworld** | Forge/Fabric | 主世界大修 | 真实地形、气候带 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Regions Unexplored** | Forge/Fabric | 未探索区域 | 新群系、独特生态 | 1.19-1.20 | ⭐⭐ 新兴 |
| **Atmospheric** | Forge | 大气群系 | 新群系、雾效、粒子 | 1.16.5-1.20 | ⭐⭐ |
| **Environmental** | Forge | 环境改进 | 新生物、群系细节 | 1.16.5-1.20 | ⭐⭐ |
| **Upgrade Aquatic** | Forge | 海洋改进 | 海带、海马、海洋生态 | 1.16.5-1.20 | ⭐⭐ |
| **Wyrmroost** | Forge | 龙类生物 | 可驯服龙、骑乘、繁殖 | 1.16.5 | ⭐⭐ 龙主题 |
| **Rats** | Forge | 老鼠模组 | 驯服老鼠、自动化、瘟疫 | 1.12.2-1.20 | ⭐⭐ 趣味向 |
| **Citadel** | Forge | 依赖库 | Alex's Mobs等前置 | 1.16.5-1.20 | ⭐⭐⭐ 基础设施 |
| **GeckoLib** | Forge/Fabric | 动画库 | 模组生物动画 | 1.12.2-1.20 | ⭐⭐⭐ 基础设施 |

---

## 七、存储/物流类模组

| 模组名 | 加载器 | 核心内容 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Applied Energistics 2 (AE2)** | Forge | 数字存储网络 | 频道、分子装配、空间塔 | 1.12.2-1.20 | ⭐⭐⭐ 终极存储 |
| **Refined Storage** | Forge | 简单存储网络 | 无线、合成、简单配置 | 1.12.2-1.20 | ⭐⭐ 入门替代 |
| **Storage Drawers** | Forge | 抽屉存储 | 量化、控制器、压缩 | 1.12.2-1.20 | ⭐⭐⭐ 经典方案 |
| **Sophisticated Storage** | Forge | 高级存储 | 升级、自动化、展示 | 1.16.5-1.20 | ⭐⭐ 现代方案 |
| **Iron Chests** | Forge/Fabric | 铁箱子升级 | 铜/铁/金/钻石/黑曜石箱子 | 1.12.2-1.20 | ⭐⭐⭐ 经典升级 |
| **Expanded Storage** | Forge/Fabric | 箱子扩展 | 多种大容量箱子 | 1.16.5-1.20 | ⭐⭐ |
| **Tom's Simple Storage** | Forge/Fabric | 简单存储 | 远程访问、简单网络 | 1.16.5-1.20 | ⭐⭐ 轻量方案 |
| **Simple Storage Network** | Forge | 简易网络 | 无频道限制、简单合成 | 1.12.2-1.20 | ⭐⭐ |
| **Pretty Pipes** | Forge | 精美管道 | 物品运输、过滤、升级 | 1.16.5-1.20 | ⭐⭐ |
| **Pipez** | Forge | 简易管道 | 物品/流体/能量/通用 | 1.16.5-1.20 | ⭐⭐ 轻量物流 |
| **XNet** | Forge | 网络控制 | 单线缆多类型传输、逻辑控制 | 1.12.2-1.20 | ⭐⭐ 技术向 |
| **Integrated Tunnels** | Forge | 集成动力学物流 | 变量控制、精准传输 | 1.12.2-1.20 | ⭐⭐ 编程向 |
| **Ender Storage** | Forge | 末影存储 | 跨维度箱子/液体/能量 | 1.12.2-1.20 | ⭐⭐⭐ 便携方案 |
| **Traveler's Backpack** | Forge/Fabric | 大容量背包 | 工具槽、睡袋、升级 | 1.16.5-1.20 | ⭐⭐⭐ 移动存储 |
| **Sophisticated Backpacks** | Forge | 高级背包 | 自动化、过滤、升级 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Carry On** | Forge/Fabric | 搬运方块/生物 | 徒手搬箱子、动物 | 1.12.2-1.20 | ⭐⭐⭐ 实用 |
| **Entangled** | Forge/Fabric | 纠缠方块 | 远程绑定、跨维度 | 1.16.5-1.20 | ⭐⭐ |
| **Compact Machines** | Forge | 空间压缩 | 在方块内建房间 | 1.12.2-1.20 | ⭐⭐ 空间利用 |

---

## 八、世界生成/地形类模组

| 模组名 | 加载器 | 核心内容 | 特色系统 | 版本支持 | 影响力 |
|:---|:---|:---|:---|:---|:---:|
| **Terralith** | Forge/Fabric | 地形生成器 | 全新地形、洞穴、结构 | 1.18-1.20 | ⭐⭐⭐ 地形神作 |
| **Biomes O' Plenty** | Forge | 生物群系扩展 | 90+新群系、子群系系统 | 1.12.2-1.20 | ⭐⭐⭐ 老牌经典 |
| **Oh The Biomes You'll Go (BYG)** | Forge/Fabric | 现代群系模组 | 80+群系、独特生态 | 1.16.5-1.20 | ⭐⭐⭐ 新兴王者 |
| **William Wythers' Overhauled Overworld** | Forge/Fabric | 主世界大修 | 真实地形、气候带、河流 | 1.16.5-1.20 | ⭐⭐⭐ 真实感 |
| **TerraForged** | Forge | 真实地形生成 | 侵蚀模拟、地质真实 | 1.16.5 | ⭐⭐ 已停更 |
| **BetterEnd** | Fabric | 末地生态大修 | 新群系、植物、材料 | 1.16.5-1.20 | ⭐⭐⭐ 维度神作 |
| **BetterNether** | Fabric | 下界生态大修 | 新森林、洞穴、材料 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Amplified Nether** | Fabric | 下界高度扩展 | y=384 下界 | 1.18-1.20 | ⭐⭐ |
| **Nullscape** | Forge/Fabric | 末地大修 | 新岛屿、地形 | 1.18-1.20 | ⭐⭐ |
| **Continents** | Forge/Fabric | 大陆地形 | 更大陆地、真实海岸 | 1.18-1.20 | ⭐⭐ |
| **Structory** | Forge/Fabric | 结构改进 | 新废墟、村庄改进 | 1.18-1.20 | ⭐⭐ |
| **Repurposed Structures** | Forge/Fabric | 结构重用 | 变种地牢、神庙 | 1.16.5-1.20 | ⭐⭐ |
| **Dungeons Plus** | Forge | 地牢扩展 | 新地牢类型 | 1.16.5-1.20 | ⭐⭐ |
| **When Dungeons Arise** | Forge/Fabric | 巨大地牢 | 大型结构、掠夺 | 1.16.5-1.20 | ⭐⭐ |
| **Better Strongholds** | Forge/Fabric | 要塞改进 | 新设计、战利品 | 1.16.5-1.20 | ⭐⭐ |
| **Better Mineshafts** | Forge/Fabric | 矿井改进 | 新结构、更丰富 | 1.16.5-1.20 | ⭐⭐ |
| **YUNG's 系列** | Forge/Fabric | 结构全面改进 | 矿井/要塞/神庙/桥梁等 | 1.16.5-1.20 | ⭐⭐⭐ 结构神作 |
| **Moog's Voyager Structures** | Forge/Fabric | 航海结构 | 船只、灯塔、港口 | 1.18-1.20 | ⭐⭐ |
| **Explorer's Compass** | Forge/Fabric | 结构指南针 | 定位最近结构 | 1.16.5-1.20 | ⭐⭐⭐ 探索必备 |
| **Nature's Compass** | Forge/Fabric | 群系指南针 | 定位特定群系 | 1.12.2-1.20 | ⭐⭐⭐ 探索必备 |

---

## 九、大型整合包代表

| 整合包名称 | 主题 | 核心模组 | 任务系统 | 难度 | 推荐版本 |
|:---|:---|:---|:---:|:---:|:---:|
| **SevTech: Ages** | 时代进化 | 自定义进度锁定、多模组联动 | ✅ 数千任务 | ⭐⭐⭐⭐⭐ 极硬核 | 1.12.2 |
| **RLCraft** | 硬核生存 | 冰与火、真实生存、恐怖生物 | ❌ 无 | ⭐⭐⭐⭐⭐ 极难 | 1.12.2 |
| **All the Mods 9 (ATM9)** | 全能综合 | 400+模组、几乎所有热门 | ✅ 引导任务 | ⭐⭐⭐ 内容过载 | 1.20.1 |
| **FTB Revelation** | 经典科技魔法 | Thermal/Mek/AE2/神秘时代 | ✅ 任务书 | ⭐⭐⭐ 平衡 | 1.12.2 |
| **Enigmatica 2/6** | 任务引导综合 | 科技魔法平衡、新手友好 | ✅ 详细任务 | ⭐⭐ 推荐入门 | 1.12.2/1.19.2 |
| **Create: Above and Beyond** | Create主题 | 机械动力为核心、自定义配方 | ✅ 任务线 | ⭐⭐⭐ 创意 | 1.16.5 |
| **SkyFactory 4** | 空岛生存 | 无中生有、自动化生产线 | ✅ 成就系统 | ⭐⭐⭐ 经典玩法 | 1.12.2 |
| **Better Minecraft** | 原版增强 | 优化+生物+维度+生活质量 | ✅ 简单引导 | ⭐⭐ 原版过渡 | 1.20.1 |
| **Vault Hunters** | 副本刷宝 | 职业技能、装备Build、副本 | ✅ RPG任务 | ⭐⭐⭐⭐ 动作RPG | 1.18.2 |
| **Dungeons, Dragons and Space Shuttles (DDSS)** | 硬核科技 | 格雷科技、极端难度 | ✅ 复杂任务 | ⭐⭐⭐⭐⭐ 专家级 | 1.12.2 |
| **Omnifactory** | 格雷科技简化 | 自动化 focus、无矿脉 | ✅ 引导 | ⭐⭐⭐⭐ 技术向 | 1.12.2 |
| **Stoneblock 3** | 石头世界 | 石头中生存、发展科技 | ✅ 任务书 | ⭐⭐⭐ 独特玩法 | 1.18.2 |
| **Seaopolis** | 海洋城市 | 海洋生存、水下建设 | ✅ 任务线 | ⭐⭐⭐ 主题生存 | 1.16.5 |
| **Medieval Minecraft** | 中世纪RPG | 冰与火、史诗战斗、任务 | ✅ RPG任务 | ⭐⭐⭐ 角色扮演 | 1.16.5/1.20.1 |
| **Astroblock 2** | 太空生存 | 高级火箭、星系探索 | ✅ 任务书 | ⭐⭐⭐⭐ 科技向 | 1.12.2 |
| **FTB Inferno** | 下界生存 | 下界开局、极端环境 | ✅ 挑战任务 | ⭐⭐⭐⭐⭐ 极难 | 1.18.2 |
| **Sprout** | 轻量探索 | 探索 focus、低科技 | ✅ 引导 | ⭐⭐ 休闲 | 1.12.2 |
| **Life in the village 2** | 村庄生活 | 模拟殖民地、轻松生存 | ✅ 任务书 | ⭐⭐ 休闲 | 1.16.5 |

---

## 十、工具/实用类模组

| 模组名 | 加载器 | 核心功能 | 使用场景 | 版本支持 | 必备度 |
|:---|:---|:---|:---|:---|:---:|
| **Jade** | Forge/Fabric | 方块信息查看 | 查看方块/实体信息 | 1.16.5-1.20 | ⭐⭐⭐ |
| **JEI/REI/EMI** | Forge/Fabric | 配方查看 | 合成查询、物品管理 | 1.12.2-1.20 | ⭐⭐⭐ |
| **JourneyMap/Xaero's** | Forge/Fabric | 地图导航 | 探索、标记、死亡点 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Waystones** | Forge/Fabric | 传送系统 | 快速旅行、基地连接 | 1.12.2-1.20 | ⭐⭐⭐ |
| **GraveStone/Corpse** | Forge/Fabric | 死亡保护 | 防掉落、物品保护 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Traveler's Backpack** | Forge/Fabric | 大背包 | 移动存储、工具携带 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Carry On** | Forge/Fabric | 搬运方块 | 移动箱子、动物运输 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Light Overlay** | Forge/Fabric | 亮度显示 | 刷怪塔建设、照明检查 | 1.12.2-1.20 | ⭐⭐⭐ |
| **AppleSkin** | Forge/Fabric | 食物信息 | 饥饿管理、饱和度查看 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Controlling** | Forge/Fabric | 按键管理 | 冲突检查、按键搜索 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Inventory Profiles** | Fabric | 背包整理 | 一键整理、自动补货 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Mouse Tweaks** | Forge/Fabric | 鼠标优化 | 快速移动、拖拽增强 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Litematica** | Fabric | 投影辅助 | 建筑复制、设计预览 | 1.16.5-1.20 | ⭐⭐⭐ 建筑必备 |
| **MiniHUD/Tweakeroo** | Fabric | 信息HUD | 坐标、时间、种子显示 | 1.16.5-1.20 | ⭐⭐ 技术玩家 |
| **Item Scroller** | Fabric | 快速移动 | 滚轮移动物品 | 1.16.5-1.20 | ⭐⭐ |
| **ShulkerBoxTooltip** | Fabric | 潜影盒预览 | 查看内容无需放置 | 1.16.5-1.20 | ⭐⭐ |
| **Mod Menu** | Fabric | 模组管理 | 列表、配置、信息 | 1.16.5-1.20 | ⭐⭐⭐ Fabric必装 |
| **Configured** | Forge/Fabric | 游戏内配置 | 无需重启修改设置 | 1.16.5-1.20 | ⭐⭐⭐ |
| **Catalogue** | Forge | 模组菜单 | Mod Menu替代品 | 1.18-1.20 | ⭐⭐ |
| **Bad Wither No Cookie** | Forge/Fabric | 音效控制 | 禁用Boss音效 | 1.12.2-1.20 | ⭐⭐ |
| **Explorer's/Nature's Compass** | Forge/Fabric | 探索工具 | 定位结构/群系 | 1.12.2-1.20 | ⭐⭐⭐ |
| **Comforts** | Forge/Fabric | 睡眠辅助 | 睡袋、吊床 | 1.12.2-1.20 | ⭐⭐ |
| **Entangled** | Forge/Fabric | 远程绑定 | 跨维度方块交互 | 1.16.5-1.20 | ⭐⭐ |
| **Compact Machines** | Forge | 空间压缩 | 方块内建房间 | 1.12.2-1.20 | ⭐⭐ |

---

## 十一、关键术语对照表

| 术语 | 解释 | 相关模组 |
|:---|:---|:---|
| **API** | 应用程序接口，模组与游戏交互的规范 | Forge API/Fabric API |
| **Mixin** | 代码注入技术，Fabric核心 | 几乎所有Fabric模组 |
| **NBT** | 数据标签格式，存储物品/方块数据 | 命令/数据包相关 |
| **Tick** | 游戏刻，20 tick = 1秒 | 红石/优化相关 |
| **TPS** | 每秒刻数，服务器性能指标 | 优化模组 |
| **FPS** | 每秒帧数，客户端性能指标 | Sodium/OptiFine等 |
| **Lag** | 卡顿，延迟 | 优化模组 |
| **Chunk** | 区块，16x16区域 | 世界生成/优化 |
| **Biome** | 生物群系 | 群系模组 |
| **Dimension** | 维度（主世界/下界/末地） | 维度模组 |
| **Loot Table** | 战利品表 | 冒险模组 |
| **Recipe** | 合成配方 | JEI查看 |
| **Tag** | 标签，物品分类系统 | 数据包/模组开发 |
| **Ore Dictionary** | 矿物词典（Forge）/ 标签（Fabric） | 科技模组兼容 |
| **GregTech** | 格雷科技，极端硬核科技 | GTCEu等 |
| **Expert Mode** | 专家模式，魔改配方 | 整合包常见 |
| **Kitchen Sink** | 包含几乎所有模组的整合包 | ATM系列 |
| **Quest Book** | 任务书，引导系统 | FTB Quests等 |
| **HQM** | 硬core任务模式（旧版） | 历史整合包 |
| **Skyblock** | 空岛生存 | SkyFactory等 |
| **SevTech** | 时代发展，进度锁定 | SevTech: Ages |
| **RLCraft** | 极端硬核生存 | RLCraft整合包 |

---
