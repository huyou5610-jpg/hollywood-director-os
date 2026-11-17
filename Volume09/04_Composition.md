# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume09
# Camera Engine
# File：04_Composition.md
# Priority：P9
# ============================================================

# Module

Composition Engine

---

# Purpose

Composition Engine（CE）。

负责建立 Hollywood Director OS 的电影构图系统（Cinema Composition System）。

Hollywood Director OS 认为：

摄影机决定：

从哪里看。

镜头决定：

怎么看。

而：

**构图决定观众理解什么。**

电影构图。

不是把人物放进画面。

而是：

组织信息。

控制注意力。

塑造关系。

传递情绪。

Composition 的职责。

就是建立：

**故事 → 空间 → 构图 → 视觉层次 → 观众理解**

的完整电影构图体系。

---

# Position

```text
Camera Theory

↓

Lens System

↓

Camera Movement

↓

Composition

↓

Blocking

↓

Visual Continuity

↓

Camera Validation
```

---

# Core Principle

每一次构图必须回答：

```text
观众第一眼看到什么？

↓

第二眼看到什么？

↓

画面隐藏了什么？

↓

画面表达了什么？

↓

AI 是否能够稳定生成？
```

构图。

决定观看顺序。

---

# Composition Philosophy

电影构图遵循：

```text
Story

↓

Emotion

↓

Visual Hierarchy

↓

Composition

↓

Audience
```

构图。

服务叙事。

---

# Composition Package

统一建立构图数据。

```yaml
Composition ID

Project ID

Scene ID

Shot ID

Frame Type

Subject Position

Balance

Depth

Narrative Function
```

---

# Composition Objectives

每一个构图至少承担一种职责。

```yaml
Guide Attention

Reveal Character

Clarify Space

Build Emotion

Show Relationship

Increase Suspense

Visual Balance

Narrative Focus

Symbolism

Audience Immersion
```

禁止：

没有信息价值的构图。

---

# Composition Hierarchy

统一控制层级。

```text
Story

↓

Emotion

↓

Subject

↓

Composition

↓

Audience
```

构图。

服从故事。

---

# Visual Hierarchy

统一视觉层级。

```yaml
Primary Subject

Secondary Subject

Supporting Objects

Background

Negative Space
```

保证：

观看顺序清晰。

---

# Rule of Thirds

统一三分法。

```yaml
Left Third

Center Third

Right Third

Upper Third

Lower Third
```

默认：

符合自然视觉阅读。

---

# Center Composition

中心构图。

统一设计。

```yaml
Power

Symmetry

Focus

Authority

Isolation
```

适用于：

高戏剧场景。

---

# Symmetry System

统一对称设计。

```yaml
Perfect Symmetry

Near Symmetry

Broken Symmetry

Intentional Asymmetry
```

体现：

秩序。

冲突。

变化。

---

# Leading Lines

统一引导线设计。

```yaml
Architecture

Road

Light

Character Gaze

Object Direction

Shadow
```

引导观众视线。

---

# Framing Techniques

统一框中框设计。

```yaml
Door

Window

Arch

Foreground Object

Shadow Frame

Natural Frame
```

强化主体。

---

# Negative Space

统一留白策略。

```yaml
Loneliness

Freedom

Tension

Expectation

Scale
```

留白。

也是叙事。

---

# Depth Composition

统一纵深设计。

```yaml
Foreground

Midground

Background

Atmosphere

Perspective
```

建立电影空间。

---

# Balance System

统一画面平衡。

```yaml
Symmetrical

Asymmetrical

Dynamic

Static

Weighted
```

画面。

保持稳定。

---

# Relationship Composition

人物关系构图。

统一设计。

```yaml
Close

Intimacy

Separated

Conflict

Layered

Hierarchy

Mirrored

Equality
```

空间。

表达关系。

---

# Eye Direction Mapping

统一视线方向。

```yaml
Look Into Frame

Engagement

Look Out Frame

Mystery

Cross Looking

Conflict

Shared Focus

Unity
```

视线。

组织信息。

---

# Visual Weight

统一视觉重量。

```yaml
Character

Lighting

Contrast

Movement

Color

Size
```

决定：

观众注意力。

---

# Color & Composition

颜色参与构图。

```yaml
Warm

Attention

Cold

Distance

Contrast

Focus

Harmony

Calm
```

颜色。

强化视觉结构。

---

# Camera Coordination

构图与摄影同步。

```yaml
Wide

Environment

Medium

Relationship

Close-up

Emotion

Extreme Close-up

Psychology
```

镜头。

决定构图尺度。

---

# AI Composition Constraints

针对 AI 视频。

建立：

```yaml
Stable Subject Placement

Stable Horizon

Stable Visual Hierarchy

Stable Perspective

Stable Frame Balance

Stable Composition Identity
```

避免：

AI 构图漂移。

---

# Workflow

```text
Story

↓

Emotion

↓

Subject Placement

↓

Visual Hierarchy

↓

Validation
```

构图。

来源于叙事。

---

# Composition Output

统一输出。

```yaml
Composition Map

Visual Hierarchy

Depth Strategy

Balance Rules

Attention Guide

AI Constraint
```

供：

Blocking。

Visual Continuity。

Camera Validation。

统一调用。

---

# Validation Rules

检查：

✓ 是否突出主体。

✓ 是否符合故事表达。

✓ 是否建立视觉层级。

✓ 是否保持空间逻辑。

✓ 是否强化观众注意力。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Blocking。

---

# Lock Rules

锁定：

```yaml
Visual Hierarchy

Subject Placement

Balance Rules

Depth Logic

Composition Identity
```

允许：

后续模块补充：

```yaml
Blocking

Continuity

Editing
```

禁止修改：

构图逻辑。

---

# Director Notes

自动生成。

```yaml
Composition Quality

Visual Balance

Narrative Clarity

Attention Control

Emotional Impact

AI Stability
```

供导演、摄影指导（DoP）、美术指导、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影构图。

不是：

画面很漂亮。

而是：

观众在第一秒。

就知道：

应该看哪里。

为什么看。

看完之后。

理解了什么。

因为：

电影构图。

不是装饰。

而是：

**信息设计。**

Composition Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影构图系统，为 Blocking、Visual Continuity、Camera Validation 与 Prompt Compiler 提供统一、稳定、具有电影级视觉叙事能力的构图框架。
