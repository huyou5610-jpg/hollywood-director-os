# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume10
# Lighting Engine
# File：02_Lighting_Design.md
# Priority：P10
# ============================================================

# Module

Lighting Design Engine

---

# Purpose

Lighting Design Engine（LDE）。

负责建立 Hollywood Director OS 的电影灯光设计系统（Cinema Lighting Design System）。

Hollywood Director OS 认为：

灯光理论决定：

为什么打光。

而：

**灯光设计决定如何打光。**

电影灯光。

不是简单布灯。

而是：

构建空间。

塑造人物。

控制层次。

设计情绪。

Lighting Design 的职责。

就是建立：

**故事 → 光位 → 光质 → 光比 → 灯具 → 电影表达**

的完整电影灯光设计体系。

---

# Position

```text
Lighting Theory

↓

Lighting Design

↓

Color Lighting

↓

Practical Lighting

↓

Lighting Continuity

↓

Lighting Validation
```

---

# Core Principle

每一次灯光设计必须回答：

```text
主光来自哪里？

↓

辅助光为什么存在？

↓

背景如何分离？

↓

阴影表达什么？

↓

AI 是否能够稳定生成？
```

灯光布局。

必须具有叙事意义。

---

# Lighting Design Philosophy

电影灯光设计遵循：

```text
Story

↓

Emotion

↓

Character

↓

Lighting Layout

↓

Audience
```

布光。

服务故事。

---

# Lighting Package

统一建立灯光设计数据。

```yaml
Lighting Setup ID

Project ID

Scene ID

Shot ID

Key Light

Fill Light

Back Light

Practical Light

Narrative Function
```

---

# Lighting Objectives

每一次布光至少承担一种职责。

```yaml
Reveal Face

Shape Volume

Separate Subject

Guide Attention

Build Atmosphere

Support Performance

Increase Contrast

Clarify Space

Enhance Emotion

Audience Immersion
```

禁止：

无目的布光。

---

# Lighting Hierarchy

统一控制层级。

```text
Story

↓

Emotion

↓

Character

↓

Lighting Setup

↓

Audience
```

灯位。

服从人物。

---

# Three-Point Lighting

统一三点布光。

```yaml
Key Light

Primary Illumination

Fill Light

Shadow Control

Back Light

Subject Separation
```

电影工业基础。

---

# Extended Lighting Setup

统一扩展灯位。

```yaml
Hair Light

Edge Light

Kicker

Rim Light

Eye Light

Background Light

Practical Source

Ambient Fill
```

适配复杂场景。

---

# Key Light Design

主光设计。

```yaml
Position

Height

Angle

Intensity

Hardness

Narrative Purpose
```

主光。

决定人物气质。

---

# Fill Light Strategy

辅光设计。

```yaml
Natural Fill

Bounce

Negative Fill

Soft Fill

Directional Fill
```

控制：

阴影密度。

---

# Back Light Strategy

轮廓光设计。

```yaml
Hair Separation

Shoulder Rim

Outline

Hero Light

Silhouette
```

强化主体层次。

---

# Light Ratio System

统一光比控制。

```yaml
1:1

Flat

2:1

Natural

4:1

Dramatic

8:1

High Contrast

16:1

Extreme Noir
```

光比。

决定戏剧张力。

---

# Shadow Design

统一阴影设计。

```yaml
Soft Shadow

Hard Shadow

Long Shadow

Broken Shadow

Pattern Shadow

Silhouette
```

阴影。

也是叙事。

---

# Light Quality

统一光质。

```yaml
Soft

Hard

Diffused

Specular

Directional

Ambient
```

光质。

决定人物质感。

---

# Subject Separation

主体分离策略。

```yaml
Back Light

Contrast

Color Difference

Depth

Focus

Negative Space
```

主体。

必须突出。

---

# Environment Lighting

环境布光。

```yaml
Interior

Exterior

Day

Night

Studio

Natural
```

统一空间逻辑。

---

# Camera Coordination

摄影与灯光同步。

```yaml
Lens

Exposure

Contrast

Highlight

Shadow

Dynamic Range
```

摄影。

匹配灯光设计。

---

# AI Lighting Constraints

针对 AI 视频。

建立：

```yaml
Stable Key Light

Stable Fill Ratio

Stable Shadow Direction

Stable Rim Light

Stable Exposure

Stable Lighting Layout
```

避免：

AI 光位漂移。

---

# Workflow

```text
Story

↓

Emotion

↓

Lighting Layout

↓

Exposure Check

↓

Validation
```

布光。

来源于戏剧需求。

---

# Lighting Design Output

统一输出。

```yaml
Lighting Blueprint

Light Position Map

Light Ratio

Shadow Design

Exposure Strategy

AI Constraint
```

供：

Color Lighting。

Lighting Continuity。

Lighting Validation。

统一调用。

---

# Validation Rules

检查：

✓ 主光是否合理。

✓ 光比是否符合戏剧。

✓ 阴影是否具有意义。

✓ 主体是否突出。

✓ 是否符合电影工业标准。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Color Lighting。

---

# Lock Rules

锁定：

```yaml
Lighting Layout

Key Light Logic

Light Ratio

Shadow Rules

Exposure Strategy
```

允许：

后续模块补充：

```yaml
Color

Practical Light

Continuity
```

禁止修改：

布光逻辑。

---

# Director Notes

自动生成。

```yaml
Lighting Layout Quality

Subject Separation

Shadow Control

Atmosphere Quality

Industrial Readiness

AI Stability
```

供导演、摄影指导（DoP）、灯光指导（Gaffer）、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影布光。

不是：

用了多少盏灯。

而是：

每一道光。

都有：

明确来源。

明确目的。

明确情绪。

明确叙事。

因为：

电影里的灯。

不是照明设备。

它是：

**导演控制观众情绪的工具。**

Lighting Design Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影灯光设计系统，为 Color Lighting、Practical Lighting、Lighting Continuity、Lighting Validation 与 Prompt Compiler 提供统一、稳定、具有电影级布光能力的灯光设计框架。
