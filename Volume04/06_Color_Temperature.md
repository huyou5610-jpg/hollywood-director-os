# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：06_Color_Temperature.md
# Priority：P4
# ============================================================

# Module

Color Temperature Engine

---

# Purpose

Color Temperature Engine（CTE）。

负责建立 Hollywood Director OS 中完整的电影色温控制系统（Color Temperature System）。

Hollywood Director OS 认为：

色温不是白平衡。

色温不是摄影参数。

色温真正控制的是：

**观众对空间、时间、情绪与真实感的认知。**

真正优秀的电影。

观众感受到的是：

寒冷。

温暖。

孤独。

安全。

危险。

而不是：

3200K。

5600K。

---

# Position

```text
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

每一个镜头必须回答：

```text
现在是什么时间？

↓

环境属于什么温度？

↓

人物心理属于什么温度？

↓

空间应该给观众什么感觉？

↓

色温是否强化故事？
```

如果色温只是技术正确。

没有叙事意义。

则失败。

---

# Color Temperature Package

建立统一数据。

```yaml
Color Temperature ID

Scene ID

Shot ID

White Balance Strategy

Primary Temperature

Secondary Temperature

Color Contrast

Narrative Purpose
```

---

# Temperature Hierarchy

建立控制层级。

```text
Story

↓

Emotion

↓

Environment

↓

Light Source

↓

Color Temperature
```

色温永远服从：

故事。

---

# Temperature Categories

统一分类。

```yaml
Warm

Neutral Warm

Neutral

Neutral Cool

Cool

Extreme Cool

Mixed Lighting
```

每个镜头。

只能拥有：

一个 Primary Temperature。

---

# Natural Temperature Mapping

真实环境。

对应色温。

```yaml
Sunrise

Warm

Morning

Neutral Warm

Noon

Neutral

Cloudy

Cool

Blue Hour

Cool

Moonlight

Cold Blue

Fire

Warm Orange

Candle

Amber

Snow

Cool Reflection
```

必须符合：

自然规律。

---

# Practical Light Temperature

真实光源。

统一定义。

```yaml
Candle

Warm

Incandescent

Warm

Halogen

Neutral Warm

LED Daylight

Neutral

LED Cool

Cool

TV

Cool Blue

Phone

Neutral Cool

Neon

Variable
```

禁止：

同一种灯。

色温随机变化。

---

# Emotional Temperature

情绪对应色温。

```yaml
Love

Warm

Family

Warm

Safety

Neutral Warm

Loneliness

Cool

Fear

Cold

Power

Neutral

Mystery

Mixed

Memory

Soft Warm

Death

Desaturated Cool
```

色温。

强化情绪。

---

# Character Temperature

人物色温。

统一管理。

```yaml
Healthy

Warm Neutral

Ill

Cool

Hero

Balanced

Villain

Directional Contrast

Memory

Warm Diffusion
```

人物。

不能脱离环境。

---

# Mixed Lighting

允许：

混合色温。

例如：

```yaml
Window Daylight

+

Warm Table Lamp

Moonlight

+

Fire

Street Light

+

Neon
```

必须：

具有真实来源。

---

# Color Contrast

建立冷暖关系。

```yaml
Warm Subject

Cool Background

Cool Subject

Warm Background

Balanced

Monochrome
```

形成：

视觉层级。

---

# White Balance Strategy

统一白平衡。

```yaml
Natural

Warm Bias

Cool Bias

Neutral Lock

Stylized
```

整个 Sequence。

保持一致。

---

# Time Progression

随着时间。

色温自动变化。

```text
Morning

↓

Warm

↓

Neutral

↓

Golden

↓

Blue Hour

↓

Night
```

禁止：

时间推进。

色温不变。

---

# Weather Influence

天气影响色温。

```yaml
Sunny

Neutral

Cloudy

Cool

Rain

Cool

Fog

Neutral Cool

Snow

Cool Reflection
```

必须：

同步变化。

---

# Environmental Reflection

环境反射。

影响色温。

```yaml
Forest

Green Bounce

Ocean

Blue Bounce

Desert

Warm Bounce

Concrete

Neutral

Snow

Cool Fill
```

增强：

真实感。

---

# Skin Tone Protection

人物肤色。

建立保护。

```yaml
Natural Skin

Hero Skin

Beauty Skin

Weathered Skin
```

禁止：

肤色漂移。

---

# AI Temperature Constraints

针对 AI 视频。

增加：

```yaml
Stable White Balance

Stable Temperature

Stable Skin Tone

Stable Color Contrast

Stable Mixed Lighting

Stable Reflection
```

避免：

AI 自动变色。

---

# Temperature Output

最终输出。

```yaml
Primary Temperature

Secondary Temperature

White Balance Strategy

Mixed Lighting Profile

Color Contrast

Skin Tone Profile

Environmental Reflection

AI Constraint
```

供：

Practical Lights。

Color Pipeline。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 色温是否符合剧情。

✓ 是否符合时间。

✓ 是否符合天气。

✓ 是否符合真实光源。

✓ 肤色是否稳定。

✓ 冷暖关系是否合理。

✓ AI 是否稳定生成。

任何失败。

禁止进入：

Practical Lights Engine。

---

# Lock Rules

锁定：

```yaml
Primary Temperature

White Balance

Color Contrast

Skin Tone Strategy

Temperature Continuity
```

允许：

后续模块补充：

```yaml
Camera Kelvin

LUT

ACES Profile

Display Transform

HDR Tone Mapping
```

禁止修改：

色温叙事逻辑。

---

# Director Notes

自动生成。

```yaml
Temperature Score

Skin Tone Accuracy

Warm/Cool Balance

Mixed Light Quality

Narrative Support

AI Temperature Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

色温不是数字。

而是情绪。

观众不会记住：

5600K。

他们会记住：

阳光很温暖。

房间很冷。

火焰令人安心。

月光令人孤独。

Color Temperature Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的电影色温系统，为 Practical Lights、Color Pipeline、HDR Workflow 与 Prompt Compiler 提供统一、稳定且具有叙事能力的色彩温度基础。

# End of File

# Next File

Volume04 / File：07_Practical_Lights.md