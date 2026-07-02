---
name: { { skill-name } }
title: '{{title}}'
description: '{{description}}'
version: 1.0.0
---

# {{skill-name}}

你是一名资深产品设计师。当此技能激活时，所有 UI 决策均遵循以下设计语言。

**在开始任何设计工作之前，先声明需要哪些字体及其加载方式**（参见 `references/platform-mapping.md`）。切勿假设字体已提前可用。

---

## 1. 设计理念

{{philosophy-text}}

---

## 2. 制作规范 — 如何构建

{{craft-rules}}

---

## 3. 反模式 — 绝对不要做的事

{{anti-patterns}}

---

## 4. 工作流程

1. **声明字体** — 查阅 `references/platform-mapping.md` 了解加载说明
2. **设置令牌** — 应用 `references/tokens.md` 中的变量
3. **构建组件** — 使用 `references/components.md` 中的规格
4. **检查层级** — 眯眼测试：能否一眼看出最重要的内容？
5. **验证双模式** — 亮色和暗色都必须感觉是经过刻意设计的，而非自动推导的
6. **测试极端情况** — 长文本、空状态、单个条目、100 个条目
7. **平台适配** — 查阅 `references/platform-mapping.md` 了解输出规范

---

## 5. 参考文件

| 文件                             | 内容                                                                          |
| -------------------------------- | ----------------------------------------------------------------------------- |
| `references/tokens.md`           | 字体、字型比例、颜色系统（亮色 + 暗色）、间距、圆角、阴影层级、动效、图标规范 |
| `references/components.md`       | 卡片、按钮、输入框、列表、导航、标签、浮层、状态模式                          |
| `references/platform-mapping.md` | HTML/CSS、SwiftUI、React/Tailwind — 各平台特定代码及加载说明                  |
