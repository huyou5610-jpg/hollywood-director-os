# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume10
# Lighting Engine
# File：03_Color_Lighting.md
# Priority：P10
# ============================================================

# Module

Color Lighting Engine

---

# Purpose

Color Lighting Engine（CLE）。

负责建立 Hollywood Director OS 的电影色彩灯光系统（Cinema Color Lighting System）。

Hollywood Director OS 认为：

布光决定：

光来自哪里。

而：

**色彩决定观众感受到什么。**

电影色彩。

不是为了漂亮。

而是：

塑造情绪。

表达时间。

区分空间。

强化角色。

建立电影风格。

Color Lighting 的职责。

就是建立：

**故事 → 色温 → 色彩 → 情绪 → 风格 → 电影表达**

的完整电影色彩灯光体系。

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

每一次色彩灯光设计必须回答：

```text
为什么使用这种颜色？

↓

色温表达什么？

↓

人物因此发生什么变化？

↓

观众感受到什么？

↓

AI 是否能够稳定生成？
```

色彩。

必须服务叙事。

---

# Color Lighting Philosophy

电影色彩遵循：

```text
Story

↓

Emotion

↓

Lighting

↓

Color

↓

Audience
```

颜色。

塑造情绪。

---

# Color Package

统一建立色彩灯光数据。

```yaml
Color ID

Project ID

Scene ID

Shot ID

Color Palette

Color Temperature

Dominant Color

Accent Color

Narrative Function
```

---

# Color Objectives

每一种颜色至少承担一种职责。

```yaml
Reveal Emotion

Define Time

Separate Space

Support Character

Guide Attention

Increase Contrast

Build Atmosphere

Visual Identity

Narrative Focus

Audience Immersion
```

禁止：

没有叙事意义的颜色。

---

# Color Hierarchy

统一控制层级。

```text
Story

↓

Emotion

↓

Lighting

↓

Color

↓

Audience
```

色彩。

服从情绪。

---

# Color Temperature System

统一色温标准。

```yaml
1800K

Candle

2700K

Warm Interior

3200K

Tungsten

4500K

Neutral

5600K

Daylight

6500K

Cool Daylight

8000K

Blue Atmosphere
```

统一工业标准。

---

# Emotional Color Mapping

颜色对应情绪。

```yaml
Warm Orange

Comfort

Golden

Hope

Blue

Loneliness

Green

Uncertainty

Red

Danger

Purple

Mystery

White

Purity

Black

Fear
```

颜色。

表达心理。

---

# Color Contrast Strategy

统一冷暖关系。

```yaml
Warm vs Cool

Emotional Conflict

Complementary

Visual Focus

Analogous

Harmony

Monochrome

Minimalism
```

色彩。

组织画面。

---

# Dominant Color Rules

统一主色策略。

```yaml
Single Dominant

Dual Balance

Triadic Palette

Accent Highlight

Neutral Base
```

主色。

建立风格。

---

# Character Color Lighting

角色灯光色彩。

```yaml
Hero

Warm Natural

Villain

Cold Contrast

Mystery

Low Saturation

Memory

Soft Warm

Dream

Pastel Glow
```

人物。

拥有独立光色。

---

# Environmental Color

环境色彩。

```yaml
Sunrise

Golden

Sunset

Amber

Night

Blue

Rain

Green Blue

Fire

Orange

Snow

Cool White
```

环境。

影响情绪。

---

# Color Rhythm

统一色彩节奏。

```yaml
Neutral

↓

Warm

↓

Peak Saturation

↓

Desaturation

↓

Transition
```

颜色。

具有节奏。

---

# Color Separation

主体色彩分离。

```yaml
Hue Difference

Saturation Difference

Brightness Difference

Temperature Difference

Contrast Difference
```

主体。

保持突出。

---

# Color Harmony

统一配色原则。

```yaml
Complementary

Split Complementary

Triadic

Analogous

Monochromatic

Neutral Accent
```

保持：

电影级统一。

---

# Camera Coordination

摄影与色彩同步。

```yaml
Exposure

White Balance

Highlight Roll-off

Shadow Tone

Contrast

Dynamic Range
```

摄影。

忠实呈现色彩设计。

---

# AI Color Constraints

针对 AI 视频。

建立：

```yaml
Stable Color Temperature

Stable White Balance

Stable Saturation

Stable Hue

Stable Contrast

Stable Palette Identity
```

避免：

AI 色彩漂移。

---

# Workflow

```text
Story

↓

Emotion

↓

Color Design

↓

Palette Validation

↓

AI Optimization
```

色彩。

来源于戏剧需求。

---

# Color Lighting Output

统一输出。

```yaml
Color Palette

Temperature Strategy

Emotion Mapping

Contrast Design

Visual Identity

AI Constraint
```

供：

Practical Lighting。

Lighting Continuity。

Lighting Validation。

统一调用。

---

# Validation Rules

检查：

✓ 色彩是否符合情绪。

✓ 色温是否合理。

✓ 配色是否统一。

✓ 是否突出主体。

✓ 是否符合电影风格。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Practical Lighting。

---

# Lock Rules

锁定：

```yaml
Color Palette

Temperature Rules

Emotion Mapping

Contrast Strategy

Visual Identity
```

允许：

后续模块补充：

```yaml
Practical Light

Continuity

Validation
```

禁止修改：

色彩语言。

---

# Director Notes

自动生成。

```yaml
Color Quality

Emotional Accuracy

Palette Consistency

Visual Impact

Industrial Readiness

AI Stability
```

供导演、摄影指导（DoP）、调色师（Colorist）、灯光指导（Gaffer）、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影色彩。

不是：

颜色鲜艳。

而是：

每一种颜色。

都让观众。

更接近人物。

更理解情绪。

更相信故事。

因为：

电影中的颜色。

不是装饰。

它是：

**情绪的光。**

Color Lighting Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影色彩灯光系统，为 Practical Lighting、Lighting Continuity、Lighting Validation 与 Prompt Compiler 提供统一、稳定、具有电影级色彩叙事能力的灯光色彩框架。
