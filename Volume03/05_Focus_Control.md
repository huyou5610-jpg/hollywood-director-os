# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：05_Focus_Control.md
# Priority：P3
# ============================================================

# Module

Focus Control Engine

---

# Purpose

Focus Control Engine（FCE）。

负责建立真人电影摄影中的焦点控制系统（Focus Language）。

Hollywood Director OS 认为：

对焦不是技术。

而是一种叙事语言。

真正决定观众注意力的。

不是镜头。

不是灯光。

而是：

**焦点。**

Focus 的职责只有一个：

**决定观众此刻必须看什么。**

---

# Position

```
Director Engine

↓

Cinematography Core

↓

Lens System

↓

Camera Movement

↓

Composition System

↓

Depth & Layer

↓

Focus Control

↓

Exposure System

↓

Lighting Engine
```

---

# Core Principle

每一个镜头必须回答：

```
观众现在应该看谁？

↓

什么时候改变焦点？

↓

为什么改变焦点？

↓

焦点变化是否推动故事？

↓

是否符合角色心理？
```

如果焦点变化没有叙事意义。

禁止变焦。

---

# Focus Package

建立统一数据。

```yaml
Focus ID

Shot ID

Primary Focus

Secondary Focus

Focus Distance

Focus Transition

Narrative Purpose
```

---

# Focus Hierarchy

建立四层控制。

```text
Story

↓

Performance

↓

Attention

↓

Focus
```

焦点永远服从：

故事。

---

# Focus Categories

统一分类。

```yaml
Single Focus

Dual Focus

Rack Focus

Deep Focus

Soft Focus

Selective Focus

Split Focus
```

每一个镜头。

只能存在：

一个 Primary Focus。

---

# Narrative Purpose

焦点必须拥有目的。

```yaml
Reveal Character

Reveal Object

Reveal Emotion

Reveal Relationship

Hide Information

Shift Attention

Build Suspense

Guide Audience
```

---

# Primary Focus

建立唯一主体。

```yaml
Character

Object

Environment

Action

Eye

Hand

Face
```

任何时刻。

只能存在一个：

Primary Focus。

---

# Secondary Focus

记录备用焦点。

例如：

```yaml
Background Character

Weapon

Phone

Door

Mirror

Vehicle
```

只有：

Rack Focus。

允许切换。

---

# Focus Transition

建立焦点变化。

```yaml
Static

Slow Rack

Fast Rack

Delayed Rack

Hidden Rack
```

变化必须：

拥有导演动机。

---

# Rack Focus Logic

默认用于：

```yaml
Truth Reveal

Relationship Shift

Discovery

Psychological Change

Attention Redirect
```

禁止：

频繁拉焦。

---

# Focus Timing

记录：

```yaml
Start Focus

Transition Point

End Focus

Hold Duration
```

焦点变化。

必须配合：

演员表演。

---

# Focus Speed

统一速度。

```yaml
Slow

Natural

Fast

Instant
```

避免：

机械切换。

---

# Eye Focus Priority

真人剧默认：

```yaml
Eyes

★★★★★

Face

★★★★★

Hands

★★★★☆

Object

★★★★☆

Environment

★★★☆☆
```

人物眼睛。

永远拥有最高权重。

---

# Multi Character Focus

多人场景。

建立：

```yaml
Leader Focus

Reaction Focus

Relationship Focus
```

观众必须知道：

谁是当前主角。

---

# Deep Focus Rules

适用于：

```yaml
Large Space

Ensemble Cast

Long Take

Relationship Scene
```

所有层。

同时清晰。

但仍然存在：

视觉主次。

---

# Soft Focus Rules

仅允许：

```yaml
Dream

Memory

Flashback

Hallucination

Romantic Style
```

禁止：

普通剧情滥用。

---

# Focus Continuity

记录：

```yaml
Previous Focus

Current Focus

Next Focus
```

确保：

镜头之间。

注意力连续。

---

# AI Focus Constraints

针对 AI 视频。

增加：

```yaml
Stable Face Focus

Stable Eye Focus

Predictable Rack Focus

No Focus Flicker

No Random Blur

Consistent Subject Priority
```

避免：

AI 自动乱切焦。

---

# Attention Curve

建立观众注意力。

```text
Observe

↓

Focus

↓

Discover

↓

React

↓

Transition
```

所有 Focus。

服务：

Attention Curve。

---

# Focus Output

最终输出：

```yaml
Primary Focus

Secondary Focus

Focus Strategy

Rack Focus Plan

Focus Timing

Attention Curve

Continuity Profile

AI Focus Constraint
```

供：

Exposure。

Lighting。

Color。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ Primary Focus 是否唯一。

✓ 焦点是否符合导演意图。

✓ Rack Focus 是否具有意义。

✓ 焦点是否跟随演员。

✓ 注意力是否连续。

✓ 是否避免 AI 焦点漂移。

✓ 是否符合真人电影摄影规范。

任何失败。

禁止进入：

Exposure System。

---

# Lock Rules

锁定：

```yaml
Primary Focus

Focus Strategy

Attention Curve

Focus Timing

Rack Focus Plan
```

允许：

Lighting。

Exposure。

Color。

补充：

```yaml
对焦距离

自动对焦参数

跟焦方式

镜头呼吸补偿
```

禁止修改：

Focus Narrative。

---

# Director Notes

自动生成：

```yaml
Attention Score

Focus Stability

Rack Focus Quality

Performance Visibility

Focus Continuity

AI Focus Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正控制观众视线的。

不是摄影机。

而是焦点。

导演决定故事。

摄影决定画面。

而 Focus 决定：

**观众此刻只能看到什么。**

Focus Control Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的焦点控制系统，为 Exposure、Lighting、Color Grading 与最终 Prompt Compiler 提供稳定、连续且具有叙事价值的视觉注意力控制。

# End of File

# Next File

Volume03 / File：06_Exposure_System.md
