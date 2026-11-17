# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：00_Lighting_Core.md
# Priority：P4
# ============================================================

# Module

Lighting Core Engine

---

# Purpose

Lighting Core Engine（LCE）。

负责建立整个 Hollywood Director OS 的电影灯光语言（Lighting Language）。

Lighting Engine 并不是决定画面亮暗。

而是负责：

**利用光塑造故事、角色、空间与情绪。**

Hollywood Director OS 认为：

真正优秀的电影灯光。

不是照亮人物。

而是：

**照亮观众应该理解的信息。**

---

# Position

```text
Director Engine

↓

Cinematography Engine

↓

Lighting Core

↓

Light Motivation

↓

Key / Fill / Rim

↓

Natural Lighting

↓

Cinematic Lighting

↓

Light Continuity

↓

Color Temperature

↓

Practical Lights

↓

AI Lighting Constraints

↓

Lighting Validation
```

---

# Core Principle

每一个灯光方案必须回答：

```text
为什么这里需要光？

↓

光从哪里来？

↓

光表达什么情绪？

↓

阴影隐藏什么信息？

↓

观众为什么相信这个光源？
```

如果灯光没有故事动机。

则灯光失败。

---

# Lighting Philosophy

灯光遵循：

```text
Story

↓

Emotion

↓

Character

↓

Space

↓

Light

↓

Shadow
```

任何情况下。

光。

不能脱离故事。

---

# Lighting Package

建立统一灯光数据。

```yaml
Lighting ID

Scene ID

Shot ID

Lighting Style

Lighting Motivation

Primary Light Source

Secondary Light Source

Shadow Strategy

Narrative Purpose
```

整个 Volume04。

统一使用此 Package。

---

# Lighting Objectives

灯光必须完成至少一项任务。

```yaml
Reveal Character

Reveal Emotion

Reveal Space

Reveal Object

Guide Audience

Create Mood

Build Tension

Separate Subject

Support Composition
```

---

# Lighting Hierarchy

建立四层控制。

```text
Story

↓

Emotion

↓

Lighting Motivation

↓

Light Placement
```

禁止：

先摆灯。

再找理由。

---

# Light Sources

统一定义真实光源。

```yaml
Sun

Moon

Sky

Window

Lamp

Fire

Candle

TV

Phone

Monitor

Vehicle

Street Light

Neon

Practical Light
```

每一个灯光。

必须拥有：

Primary Source。

---

# Lighting Style

统一风格分类。

```yaml
Naturalistic

Classical Hollywood

Noir

High Key

Low Key

Realism

Stylized

Expressionistic
```

整个 Scene。

保持一致。

---

# Narrative Purpose

灯光必须服务：

```yaml
Hope

Fear

Love

Loneliness

Mystery

Power

Danger

Freedom

Isolation

Truth
```

禁止：

仅为了漂亮。

---

# Subject Priority

灯光优先级。

```yaml
Eyes

★★★★★

Face

★★★★★

Primary Subject

★★★★★

Hands

★★★★☆

Environment

★★★☆☆

Background

★★☆☆☆
```

演员。

永远优先。

---

# Shadow Philosophy

阴影承担：

```yaml
Hide

Separate

Compress

Threaten

Mystify

Balance
```

阴影不是缺光。

而是：

信息控制。

---

# Lighting Balance

建立整体平衡。

```yaml
Light Dominant

Balanced

Shadow Dominant
```

根据剧情自动决定。

---

# Spatial Lighting

建立空间照明。

```yaml
Foreground

Midground

Background
```

每一层。

都必须具有：

独立光照逻辑。

---

# Lighting Rhythm

记录光线变化。

```yaml
Static

Gradual

Progressive

Dynamic

Flash

Pulse
```

光线变化。

必须具有：

戏剧原因。

---

# Visual Consistency

统一控制。

```yaml
Direction

Intensity

Quality

Color

Contrast

Shadow Density
```

保证：

摄影连续。

---

# AI Lighting Foundation

针对 AI 视频。

建立基础约束。

```yaml
Stable Light Source

Stable Shadow

Stable Contrast

Stable Exposure

Stable Reflection

Stable Subject Lighting
```

避免：

AI 灯光漂移。

---

# Lighting Workflow

```text
Director Package

↓

Determine Emotion

↓

Determine Motivation

↓

Determine Source

↓

Determine Style

↓

Determine Shadow

↓

Determine Balance

↓

Validate
```

禁止跳步。

---

# Lighting Output

统一输出。

```yaml
Lighting Style

Lighting Motivation

Primary Light

Secondary Light

Shadow Strategy

Lighting Balance

Spatial Lighting

Narrative Purpose

AI Constraint
```

供后续所有灯光模块调用。

---

# Validation Rules

检查：

✓ 是否具有真实光源。

✓ 是否符合导演意图。

✓ 是否强化角色表演。

✓ 是否保持空间真实。

✓ 是否拥有统一风格。

✓ 是否符合 AI 连续生成。

任何失败。

禁止进入：

Light Motivation Engine。

---

# Lock Rules

锁定：

```yaml
Lighting Style

Lighting Motivation

Primary Source

Narrative Purpose

Shadow Strategy
```

允许后续模块补充：

```yaml
Light Position

Light Size

Intensity

Diffusion

Practical Units

Lighting Ratio
```

禁止修改：

灯光叙事逻辑。

---

# Final Principle

Hollywood Director OS 中。

摄影决定：

观众从哪里看。

灯光决定：

**观众相信什么。**

每一道光。

都是故事的一部分。

每一片阴影。

都是导演故意保留的信息。

Lighting Core Engine 输出的是一套符合好莱坞真人电影工业标准，并适配 AI 视频生成的统一灯光核心系统，为后续 Light Motivation、三点布光、自然光、影视灯光设计与 Prompt Compiler 提供稳定可靠的灯光基础。

# End of File

# Next File

Volume04 / File：01_Light_Motivation.md
