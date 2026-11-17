# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：01_Director_Intent.md
# Priority：P2
# ============================================================

# Module

Director Intent Engine

---

# Purpose

Director Intent Engine（DIE）。

负责把 Director Core 输出的导演目标（Director Goal），转换成整个制作系统可以执行的导演意图（Director Intent）。

导演不会直接思考：

"我要推镜。"

导演首先思考：

"我要让观众感受到压迫。"

因此。

Director Intent 是所有摄影、表演、灯光、剪辑的共同源头。

---

# Position

```
Director Core

↓

Director Intent Engine

↓

Shot Design

↓

Camera Language

↓

Blocking

↓

Lighting

↓

Editing
```

---

# Core Principle

导演意图不是镜头。

导演意图回答的是：

```
我要让观众感受到什么？

↓

我要表达什么？

↓

我要隐藏什么？

↓

我要强调什么？

↓

我要什么时候揭示？
```

所有镜头。

都是 Intent 的表达工具。

---

# Director Intent Package

每个 Scene 建立唯一 Intent。

```yaml
Intent ID

Scene ID

Scene Objective

Director Goal

Audience Emotion

Narrative Focus

Visual Focus
```

---

# Intent Hierarchy

导演意图采用三级结构。

```
Primary Intent

↓

Secondary Intent

↓

Supporting Intent
```

例如：

```yaml
Primary

Build Suspense

Secondary

Hide Killer

Supporting

Increase Audience Curiosity
```

任何 Scene。

只能存在：

一个 Primary Intent。

---

# Intent Categories

系统统一分类。

```yaml
Reveal

Hide

Pressure

Isolation

Hope

Fear

Romance

Mystery

Comedy

Power

Weakness

Chaos

Order

Freedom

Control
```

允许组合。

必须指定：

Primary Intent。

---

# Audience Experience

建立观众体验曲线。

```yaml
Audience Entry

Audience Build

Audience Peak

Audience Exit
```

例如：

```
Safe

↓

Uneasy

↓

Fear

↓

Relief
```

所有导演决策。

服务于这条曲线。

---

# Narrative Focus

定义：

这一场戏真正关注什么。

```yaml
Character

Relationship

Information

Conflict

Environment

Action

Emotion
```

摄影机。

不得偏离 Focus。

---

# Information Strategy

导演决定：

信息什么时候给观众。

```yaml
Known

Hidden

Delayed

Revealed

Misleading
```

例如：

凶手。

可以：

存在。

但：

暂不展示。

---

# Emotional Strategy

定义：

情绪推进方式。

```yaml
Slow Burn

Sudden Shock

Gradual Relief

Continuous Pressure

Emotional Release
```

后续：

摄影。

音乐。

剪辑。

全部继承。

---

# Visual Strategy

建立：

视觉表达目标。

```yaml
Isolation

Crowding

Symmetry

Asymmetry

Negative Space

Depth

Foreground Blocking

Backlight

Silhouette
```

这些不是摄影技巧。

而是导演表达。

---

# Performance Strategy

定义演员重点。

```yaml
Dialogue First

Silence First

Reaction First

Eye Contact

Micro Expression

Body Language
```

例如：

本 Scene。

重点不是对白。

而是：

沉默。

---

# Camera Strategy Hint

Director Intent 不设计镜头。

只给摄影目标。

例如：

```yaml
Observe

Follow

Reveal

Hide

Witness

Confront

Distance

Intimacy
```

Camera Engine。

自行实现。

---

# Editing Strategy Hint

定义剪辑方向。

```yaml
Fast Rhythm

Slow Rhythm

Long Take

Reaction Cut

Parallel Editing

Invisible Editing
```

不是具体剪辑。

只是导演要求。

---

# Lighting Strategy Hint

导演告诉灯光：

```yaml
Natural

Stylized

High Contrast

Soft

Cold

Warm

Motivated Light
```

Lighting Engine。

负责执行。

---

# Blocking Strategy Hint

导演告诉演员：

```yaml
Approach

Separate

Surround

Escape

Corner

Protect

Observe
```

Blocking Engine。

设计具体走位。

---

# Director Priority Matrix

系统自动生成：

```yaml
Performance

★★★★★

Story

★★★★★

Emotion

★★★★★

Camera

★★★★☆

Lighting

★★★☆☆

Environment

★★★☆☆

FX

★★☆☆☆
```

保证：

导演永远先关注故事。

不是特效。

---

# Conflict Resolution

如果：

多个 Intent 冲突。

统一采用：

```
Story

>

Performance

>

Emotion

>

Camera

>

Lighting

>

FX
```

故事优先。

---

# Director Intent Output

最终输出：

```yaml
Primary Intent

Audience Curve

Narrative Focus

Information Strategy

Emotion Strategy

Visual Strategy

Performance Strategy

Camera Hint

Blocking Hint

Lighting Hint

Editing Hint

Priority Matrix
```

供：

Shot Design Engine。

统一读取。

---

# Validation Rules

检查：

✓ Primary Intent 唯一。

✓ Audience Emotion 完整。

✓ Narrative Focus 明确。

✓ Information Strategy 合理。

✓ Performance Priority 存在。

✓ Camera Hint 存在。

✓ Story Goal 一致。

✓ Scene Objective 一致。

任何失败。

禁止进入 Shot Design。

---

# Lock Rules

锁定：

```yaml
Primary Intent

Narrative Focus

Audience Curve

Information Strategy
```

允许后续模块补充：

```yaml
具体镜头

具体焦段

具体灯位

具体剪辑点
```

禁止修改导演意图。

---

# Final Principle

Director Intent Engine 是整个 Hollywood Director OS 的导演大脑。

它决定的不是镜头怎么拍。

而是：

**为什么这样拍。**

镜头只是语言。

导演意图才是真正的思想。

Hollywood Director OS 的所有摄影、灯光、表演、剪辑，都必须忠实执行 Director Intent，而不是各自独立决策。

# End of File

# Next File

Volume02 / File：02_Shot_Design.md
