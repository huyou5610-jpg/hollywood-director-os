# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume05
# Color Pipeline Engine
# File：02_Color_Palette.md
# Priority：P5
# ============================================================

# Module

Color Palette Engine

---

# Purpose

Color Palette Engine（CPE）。

负责建立 Hollywood Director OS 的电影色彩调色板系统（Cinema Color Palette System）。

Hollywood Director OS 认为：

电影中的颜色不是随机出现。

每一种颜色。

都应该拥有：

**叙事职责。**

真正优秀的电影调色板。

不会拥有很多颜色。

而是拥有：

**足够精准的颜色。**

Color Palette 的职责。

就是建立整个电影世界的颜色秩序。

---

# Position

```text
Color Pipeline Core

↓

Color Science

↓

Color Palette

↓

Color Script

↓

Color Emotion

↓

LUT System

↓

HDR Workflow

↓

ACES Pipeline

↓

AI Color Constraints

↓

Color Validation
```

---

# Core Principle

每一个调色板必须回答：

```text
故事属于什么颜色？

↓

角色属于什么颜色？

↓

环境属于什么颜色？

↓

颜色之间是否具有关系？

↓

AI 是否能够稳定重建？
```

如果颜色没有组织。

Color Palette 失败。

---

# Color Palette Package

统一建立数据。

```yaml
Palette ID

Project ID

Scene ID

Shot ID

Primary Palette

Secondary Palette

Accent Palette

Narrative Purpose
```

---

# Palette Hierarchy

建立颜色层级。

```text
Story

↓

Emotion

↓

Character

↓

Environment

↓

Lighting

↓

Palette

↓

Shot
```

颜色永远服务故事。

---

# Palette Structure

统一结构。

```yaml
Primary Color

Secondary Color

Accent Color

Neutral Color

Reserved Color
```

每个 Scene。

保持统一比例。

---

# Primary Palette

负责：

```yaml
World Identity

Environment

Mood

Narrative Tone
```

通常占：

```yaml
60%
```

---

# Secondary Palette

负责：

```yaml
Character

Architecture

Props

Visual Balance
```

通常占：

```yaml
30%
```

---

# Accent Palette

负责：

```yaml
Attention

Danger

Love

Power

Story Turning Point
```

通常占：

```yaml
10%
```

Accent Color。

禁止滥用。

---

# Neutral Palette

统一中性色。

```yaml
White

Gray

Black

Brown

Stone

Concrete
```

承担：

视觉缓冲。

---

# Reserved Color

建立保留色。

例如：

```yaml
Red

Only Death

Gold

Only Hope

Blue

Only Isolation

Green

Only Nature

Purple

Only Royalty
```

禁止：

随意使用。

---

# Palette Categories

统一风格。

```yaml
Warm

Cool

Monochrome

Earth Tone

Pastel

Muted

High Contrast

Low Saturation

Neo Noir

Technicolor
```

整个 Sequence。

保持一致。

---

# Character Palette

每位角色建立：

```yaml
Primary

Secondary

Accent

Transformation Palette
```

颜色变化。

对应人物成长。

---

# Environment Palette

环境建立：

```yaml
Interior

Exterior

Urban

Nature

Industrial

Historical

Fantasy
```

空间拥有独立配色。

---

# Costume Synchronization

服装同步。

```yaml
Hero

Supporting

Crowd

Enemy

Background
```

避免：

颜色冲突。

---

# Prop Synchronization

道具颜色。

统一管理。

```yaml
Weapon

Vehicle

Furniture

Technology

Food

Book
```

强化：

视觉识别。

---

# Lighting Synchronization

调色板同步：

```yaml
Lighting Color

Practical Light

Atmosphere

Reflection
```

保持：

光色一致。

---

# Emotional Mapping

颜色映射情绪。

```yaml
Warm Gold

Hope

Amber

Home

Cool Blue

Loneliness

Green

Nature

Crimson

Conflict

Purple

Power

Gray

Depression
```

颜色强化故事。

---

# Palette Transition

允许颜色变化。

```yaml
Static

Gradual Shift

Narrative Shift

Character Shift

Emotional Shift
```

变化必须：

具有剧情依据。

---

# Saturation Strategy

统一饱和度。

```yaml
Low

Medium

High

Stylized

Selective
```

禁止：

随机变化。

---

# Contrast Strategy

颜色反差。

```yaml
Complementary

Analogous

Triadic

Split Complementary

Monochrome
```

建立：

视觉秩序。

---

# AI Palette Constraints

针对 AI 视频。

建立：

```yaml
Stable Hue

Stable Saturation

Stable Palette Ratio

Stable Accent Color

Stable Skin Tone

Stable Environment
```

避免：

AI 自动改变主色。

---

# Palette Output

统一输出。

```yaml
Primary Palette

Secondary Palette

Accent Palette

Neutral Palette

Reserved Color

Contrast Strategy

Transition Rule

AI Constraint
```

供：

Color Script。

Color Emotion。

LUT。

统一调用。

---

# Validation Rules

检查：

✓ 主色是否统一。

✓ Accent 是否克制。

✓ 是否符合角色设定。

✓ 是否符合环境。

✓ 是否强化情绪。

✓ 是否支持 AI 连续生成。

任何失败。

禁止进入：

Color Script Engine。

---

# Lock Rules

锁定：

```yaml
Primary Palette

Secondary Palette

Accent Palette

Reserved Color

Palette Ratio
```

允许：

后续模块补充：

```yaml
Film LUT

HDR Mapping

Display Transform

Creative Grade
```

禁止修改：

调色板逻辑。

---

# Director Notes

自动生成。

```yaml
Palette Consistency

Visual Identity

Character Recognition

Environment Harmony

Narrative Support

AI Palette Stability
```

供导演、美术指导与调色师审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影调色板。

不是颜色丰富。

而是颜色精准。

观众不会记住：

用了多少种颜色。

他们会记住：

**那个世界一直是金色的。**

**那个角色一直穿着蓝色。**

**那一抹红色出现时，故事开始改变。**

Color Palette Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo 等 AI 视频生成模型的统一电影调色板系统，为 Color Script、Color Emotion、LUT System、HDR Workflow 与 Prompt Compiler 提供稳定、统一、具有叙事能力的色彩结构。

# End of File

# Next File

Volume05 / File：03_Color_Script.md