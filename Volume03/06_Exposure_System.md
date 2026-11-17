# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：06_Exposure_System.md
# Priority：P3
# ============================================================

# Module

Exposure System Engine

---

# Purpose

Exposure System Engine（ESE）。

负责建立真人电影摄影中的曝光控制系统（Exposure Language）。

Hollywood Director OS 认为：

曝光不是让画面变亮。

曝光不是摄影参数。

曝光真正控制的是：

**观众能看到多少信息。**

光。

永远服务故事。

暗。

也是故事的一部分。

---

# Position

```text
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

```text
观众应该看到什么？

↓

哪些信息应该隐藏？

↓

亮部代表什么？

↓

暗部代表什么？

↓

曝光是否强化了故事？
```

如果曝光只是技术正确。

而没有叙事意义。

曝光失败。

---

# Exposure Package

建立统一曝光数据。

```yaml
Exposure ID

Shot ID

Exposure Strategy

Dynamic Range

Key Exposure

Shadow Level

Highlight Level

Narrative Purpose
```

---

# Exposure Hierarchy

建立四层逻辑。

```text
Story

↓

Emotion

↓

Lighting Intent

↓

Exposure
```

曝光。

永远最后决定。

---

# Exposure Categories

统一曝光类型。

```yaml
High Key

Low Key

Natural

Contrast

Silhouette

Backlight

Mixed Lighting

Motivated Lighting
```

每一个镜头。

只能拥有：

Primary Exposure。

---

# Narrative Purpose

曝光必须拥有戏剧目的。

```yaml
Reveal Truth

Hide Information

Create Suspense

Increase Isolation

Romantic Atmosphere

Psychological Pressure

Power Contrast

Environmental Mood
```

---

# Dynamic Range

建立宽容度。

```yaml
Low

Medium

High

Extreme
```

根据：

摄影风格。

自动决定。

---

# Highlight Strategy

亮部承担：

```yaml
Attention

Hope

Power

Truth

Heaven

Memory
```

禁止：

亮部毫无意义。

---

# Shadow Strategy

暗部承担：

```yaml
Mystery

Fear

Isolation

Unknown

Hidden Object

Psychological Space
```

阴影。

必须讲故事。

---

# Exposure Priority

统一曝光权重。

```yaml
Actor Face

★★★★★

Eyes

★★★★★

Primary Subject

★★★★★

Environment

★★★★☆

Background

★★★☆☆

FX

★★☆☆☆
```

人物。

优先于环境。

---

# Skin Tone Protection

真人剧默认：

保护人物肤色。

```yaml
Face Exposure Lock

Eye Detail Lock

Skin Texture Lock
```

禁止：

人物脸部过曝。

或死黑。

---

# Contrast Design

建立反差策略。

```yaml
Soft Contrast

Balanced

High Contrast

Extreme Contrast
```

不同类型：

对应不同心理。

---

# Motivated Exposure

所有曝光必须来自：

真实光源。

例如：

```yaml
Window

Sun

Moon

Lamp

Fire

Phone

TV

Street Light
```

禁止：

无来源亮光。

---

# Interior / Exterior Balance

记录：

```yaml
Indoor

Outdoor

Mixed

Transition
```

保证：

室内外曝光连续。

---

# Day / Night Logic

建立：

```yaml
Day

Golden Hour

Blue Hour

Night

Artificial Night
```

曝光必须符合：

时间逻辑。

---

# Exposure Transition

记录：

```yaml
Previous Exposure

Current Exposure

Next Exposure
```

保证：

镜头切换。

曝光自然。

---

# HDR Strategy

支持：

```yaml
Standard

HDR Natural

HDR Cinematic
```

禁止：

HDR 炫技。

---

# AI Exposure Constraints

针对 AI 视频。

增加：

```yaml
Stable Brightness

Stable Face Exposure

No Exposure Flicker

Consistent Contrast

Consistent White Balance

Stable Highlight
```

避免：

AI 自动闪光。

亮度漂移。

---

# Exposure Output

最终输出：

```yaml
Exposure Strategy

Dynamic Range

Highlight Plan

Shadow Plan

Contrast Strategy

Skin Tone Protection

Exposure Continuity

AI Exposure Constraint
```

供：

Lighting。

Color Grading。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ Exposure 是否符合导演意图。

✓ 人物曝光是否正确。

✓ Highlight 是否具有叙事意义。

✓ Shadow 是否具有信息。

✓ Dynamic Range 是否合理。

✓ Exposure 是否连续。

✓ AI 是否能够稳定生成。

任何失败。

禁止进入：

Lighting Engine。

---

# Lock Rules

锁定：

```yaml
Exposure Strategy

Highlight Strategy

Shadow Strategy

Contrast Strategy

Exposure Continuity
```

允许：

Lighting Engine。

补充：

```yaml
ISO

Shutter

Aperture

ND Filter

Camera Profile

HDR Setting
```

禁止修改：

曝光叙事逻辑。

---

# Director Notes

自动生成：

```yaml
Exposure Score

Face Protection

Contrast Analysis

Shadow Quality

Highlight Balance

AI Exposure Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

曝光不是摄影参数。

而是导演控制信息密度的方法。

观众看到多少。

隐藏多少。

相信多少。

全部由曝光决定。

优秀电影不会让画面一直明亮。

而是让每一道光。

每一片阴影。

都拥有戏剧意义。

Exposure System Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的曝光控制系统，为 Lighting Engine、Color Pipeline 与最终 Director Execution Sheet 提供稳定可靠的曝光基础。

# End of File

# Next File

Volume03 / File：07_Camera_Continuity.md
