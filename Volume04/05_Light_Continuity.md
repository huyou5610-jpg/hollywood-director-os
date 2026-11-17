# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：05_Light_Continuity.md
# Priority：P4
# ============================================================

# Module

Light Continuity Engine

---

# Purpose

Light Continuity Engine（LCT）。

负责建立 Hollywood Director OS 中完整的灯光连续性系统（Lighting Continuity System）。

Hollywood Director OS 认为：

真正优秀的电影灯光。

观众不会注意它是否变化。

观众只会相信：

**光一直真实存在于这个世界。**

Light Continuity 的职责。

不是保持所有镜头一样。

而是：

**保证灯光变化拥有合理的时间、空间与剧情逻辑。**

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

每一次灯光变化。

必须回答：

```text
为什么发生变化？

↓

是谁导致变化？

↓

环境发生了什么？

↓

时间是否推进？

↓

观众是否相信？
```

如果灯光变化没有原因。

连续性失败。

---

# Continuity Package

建立统一数据。

```yaml
Continuity ID

Scene ID

Sequence ID

Shot ID

Lighting State

Previous State

Current State

Next State

Transition Type
```

---

# Lighting Hierarchy

建立连续性层级。

```text
Project

↓

Episode

↓

Sequence

↓

Scene

↓

Shot
```

高层定义风格。

低层执行变化。

---

# Continuity Categories

统一分类。

```yaml
Static

Natural Progression

Story Driven

Environmental

Character Driven

Practical Driven

Emotional Transition
```

每一次变化。

必须属于其中一种。

---

# Light State

记录完整灯光状态。

```yaml
Primary Source

Secondary Source

Direction

Intensity

Contrast

Color Temperature

Shadow Density

Atmosphere
```

任何镜头。

不得遗漏。

---

# Time Continuity

时间推动灯光。

```yaml
Morning

↓

Noon

↓

Afternoon

↓

Golden Hour

↓

Blue Hour

↓

Night
```

禁止：

时间跳跃。

光照不变。

---

# Weather Continuity

天气推动灯光。

```yaml
Sunny

↓

Cloudy

↓

Rain

↓

Storm

↓

Fog

↓

Snow
```

天气变化。

必须同步：

光质。

阴影。

色温。

---

# Practical Continuity

真实光源。

保持一致。

```yaml
Lamp

TV

Phone

Monitor

Fire

Street Light

Vehicle Headlight
```

例如：

```text
角色关闭台灯

↓

下一镜

房间变暗
```

禁止：

灯灭了。

画面仍然明亮。

---

# Character Driven Lighting

角色行为。

影响灯光。

例如：

```yaml
Open Curtain

Close Curtain

Enter Room

Exit Room

Open Door

Turn On TV

Light Fire
```

行为。

必须改变光线。

---

# Environmental Continuity

环境变化。

影响：

```yaml
Sun Angle

Cloud

Fog

Smoke

Dust

Reflection

Shadow Length
```

环境。

优先于摄影。

---

# Emotional Transition

允许灯光：

随情绪变化。

```yaml
Hope

↓

Warm

Fear

↓

Cold

Truth

↓

Bright

Isolation

↓

Shadow
```

必须：

循序渐进。

---

# Shot Transition

记录镜头切换。

```yaml
Cut

Match Cut

Dissolve

Fade

Long Take
```

不同切换。

允许不同灯光变化速度。

---

# Sequence Continuity

整个 Sequence。

统一：

```yaml
Lighting Style

Contrast

Shadow Logic

Mood

Color Direction
```

保证：

摄影语言统一。

---

# Shadow Continuity

统一阴影。

```yaml
Direction

Density

Edge Softness

Length

Movement
```

禁止：

阴影方向跳变。

---

# Reflection Continuity

统一反射。

```yaml
Glass

Metal

Water

Floor

Vehicle

Skin
```

反射必须：

跟随光源。

---

# Atmosphere Continuity

统一空气介质。

```yaml
Fog

Smoke

Dust

Rain

Snow

Volumetric Light
```

保证：

空间一致。

---

# AI Lighting Continuity

针对 AI 视频。

增加：

```yaml
Stable Direction

Stable Intensity

Stable Shadow

Stable Reflection

Stable Practical

Stable Atmosphere
```

避免：

AI 自动改变：

灯光方向。

亮度。

阴影。

---

# Continuity Memory

建立灯光记忆。

```yaml
Previous Lighting

Current Lighting

Next Lighting
```

自动继承：

```yaml
Source

Direction

Contrast

Shadow

Temperature
```

降低：

AI 漂移。

---

# Lighting Transition Curve

统一变化曲线。

```yaml
Hold

Ease In

Ease Out

Linear

Gradual Fade

Sudden Shift
```

变化速度。

必须符合剧情。

---

# Continuity Output

最终输出。

```yaml
Lighting State

Transition Type

Time Progress

Weather Progress

Shadow Profile

Reflection Profile

Atmosphere Profile

AI Continuity Constraint
```

供：

Color Temperature。

Practical Lights。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 光源是否连续。

✓ 时间是否连续。

✓ 天气是否连续。

✓ 阴影是否连续。

✓ Practical Light 是否一致。

✓ Atmosphere 是否一致。

✓ AI 是否稳定生成。

任何失败。

禁止进入：

Color Temperature Engine。

---

# Lock Rules

锁定：

```yaml
Lighting State

Shadow Logic

Transition Curve

Continuity Memory

Atmosphere State
```

允许：

后续模块补充：

```yaml
Color Grade

Render LUT

Exposure Fine Tune

HDR Profile
```

禁止修改：

灯光连续性逻辑。

---

# Director Notes

自动生成。

```yaml
Continuity Score

Lighting Drift Risk

Shadow Drift Risk

Reflection Stability

Atmosphere Consistency

AI Lighting Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的灯光连续性。

不是每个镜头都一样。

而是让观众始终相信：

**太阳一直在那里。**

**灯一直亮着。**

**人物一直生活在同一个世界。**

Light Continuity Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的灯光连续性系统，为 Color Temperature、Color Pipeline 与 Prompt Compiler 提供稳定、可信、连续的光照基础。

# End of File

# Next File

Volume04 / File：06_Color_Temperature.md