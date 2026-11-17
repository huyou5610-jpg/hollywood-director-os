# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：03_Natural_Lighting.md
# Priority：P4
# ============================================================

# Module

Natural Lighting Engine

---

# Purpose

Natural Lighting Engine（NLE）。

负责建立 Hollywood Director OS 中的自然光照系统（Natural Lighting System）。

Hollywood Director OS 认为：

真正优秀的电影灯光。

首先应该看起来：

**不像打过灯。**

自然光不是摄影妥协。

而是：

**最可信的电影光语言。**

Natural Lighting Engine 的目标。

是让 AI 学会：

**真实世界的光如何存在。**

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
```

---

# Core Principle

每一个自然光方案。

必须回答：

```text
太阳在哪里？

↓

天空如何影响光线？

↓

建筑如何改变光线？

↓

天气如何改变光质？

↓

观众是否相信这是自然形成的？
```

如果光线违背自然规律。

自然光失败。

---

# Natural Lighting Package

建立统一数据。

```yaml
Natural Lighting ID

Scene ID

Shot ID

Time of Day

Weather

Primary Natural Source

Secondary Bounce

Atmospheric Effect

Narrative Purpose
```

---

# Lighting Hierarchy

建立自然光控制流程。

```text
Story

↓

Environment

↓

Time

↓

Weather

↓

Natural Light

↓

Cinematic Enhancement
```

禁止：

先决定光效。

后决定天气。

---

# Natural Light Sources

统一真实来源。

```yaml
Sun

Sky

Cloud

Moon

Stars

Window

Open Door

Snow Reflection

Water Reflection

Ground Bounce
```

所有自然光。

必须来自：

真实来源。

---

# Time of Day

统一时间模型。

```yaml
Pre Dawn

Sunrise

Morning

Late Morning

Noon

Afternoon

Golden Hour

Sunset

Blue Hour

Night

Moonlight
```

每个时间段。

拥有固定光照逻辑。

---

# Sun Position

建立太阳高度。

```yaml
Low

Medium

High

Setting

Below Horizon
```

影响：

```yaml
Shadow Length

Light Direction

Contrast

Color Temperature
```

---

# Sky Conditions

天空类型。

```yaml
Clear

Partly Cloudy

Overcast

Storm

Fog

Snow
```

不同天空。

自动改变：

光质。

---

# Weather Mapping

天气影响灯光。

```yaml
Sunny

Hard Shadow

Cloudy

Soft Shadow

Rain

Low Contrast

Fog

Diffused Light

Snow

High Bounce
```

天气。

必须连续。

---

# Window Lighting

窗光分类。

```yaml
Direct Sun

Indirect Sun

North Light

South Light

East Light

West Light

Skylight
```

默认：

窗光为人物主光。

---

# Moonlight Logic

月光规则。

```yaml
Soft

Directional

Low Intensity

Blue Shift

Long Shadow
```

禁止：

夜晚出现正午效果。

---

# Ambient Light

环境光。

统一分类。

```yaml
Sky Fill

Ground Bounce

Wall Bounce

Water Reflection

Vegetation Reflection
```

提升：

真实感。

---

# Atmospheric Lighting

建立空气介质。

```yaml
Mist

Fog

Dust

Smoke

Humidity

Rain
```

增加：

空间层次。

---

# Landscape Interaction

自然环境影响。

```yaml
Forest

Mountain

Desert

Ocean

Snow Field

City
```

环境。

自动影响：

反射。

阴影。

亮度。

---

# Indoor Natural Light

室内自然光。

统一来源。

```yaml
Window

Door

Skylight

Glass Roof

Courtyard

Reflection
```

禁止：

室内均匀照亮。

---

# Outdoor Natural Light

室外自然光。

建立：

```yaml
Sun

Sky Fill

Ground Bounce

Atmospheric Perspective
```

形成：

真实户外光照。

---

# Seasonal Lighting

季节影响。

```yaml
Spring

Summer

Autumn

Winter
```

改变：

```yaml
Sun Angle

Light Duration

Atmosphere

Vegetation Reflection
```

---

# Character Integration

人物必须融入：

自然光环境。

检查：

```yaml
Face Direction

Shadow Direction

Ground Shadow

Eye Reflection

Skin Response
```

人物。

不能脱离环境。

---

# AI Natural Constraints

针对 AI 视频。

增加：

```yaml
Stable Sun Direction

Stable Shadow Length

Stable Sky Color

Stable Weather

Stable Reflection

Stable Atmospheric Effect
```

避免：

太阳跳位。

阴影漂移。

---

# Natural Lighting Output

最终输出。

```yaml
Time Profile

Weather Profile

Sun Position

Natural Source

Ambient Strategy

Atmospheric Effect

Character Integration

AI Constraint
```

供：

Cinematic Lighting。

Color Temperature。

统一调用。

---

# Validation Rules

检查：

✓ 时间是否正确。

✓ 天气是否一致。

✓ 光源是否真实。

✓ 阴影是否正确。

✓ 人物是否融入环境。

✓ Atmosphere 是否合理。

✓ AI 是否稳定生成。

任何失败。

禁止进入：

Cinematic Lighting。

---

# Lock Rules

锁定：

```yaml
Time

Weather

Natural Source

Sun Position

Ambient Strategy
```

允许：

后续模块补充。

```yaml
Artificial Enhancement

Diffusion

Negative Fill

Bounce Board

Practical Light Mix
```

禁止修改：

自然光逻辑。

---

# Director Notes

自动生成。

```yaml
Naturalism Score

Weather Accuracy

Sun Consistency

Shadow Quality

Environmental Integration

AI Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的自然光。

不是复制现实。

而是：

**提炼现实。**

观众相信。

太阳真的在那里。

云真的遮住了阳光。

风真的改变了空气。

人物真的生活在那个世界。

Natural Lighting Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的自然光系统，为后续 Cinematic Lighting、Color Temperature、Color Pipeline 与 Prompt Compiler 提供真实可信的自然光基础。

# End of File

# Next File

Volume04 / File：04_Cinematic_Lighting.md