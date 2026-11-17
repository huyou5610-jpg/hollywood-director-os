# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume10
# Lighting Engine
# File：05_Lighting_Continuity.md
# Priority：P10
# ============================================================

# Module

Lighting Continuity Engine

---

# Purpose

Lighting Continuity Engine（LCE）。

负责建立 Hollywood Director OS 的电影灯光连续性系统（Cinema Lighting Continuity System）。

Hollywood Director OS 认为：

真正优秀的电影灯光。

不是：

某一个镜头很漂亮。

而是：

**所有镜头始终属于同一个世界。**

灯光连续性。

不仅是：

亮度一致。

更是：

时间一致。

方向一致。

色彩一致。

空间一致。

情绪一致。

Lighting Continuity 的职责。

就是建立：

**镜头 → 光源 → 色温 → 光位 → 阴影 → 时间 → 连续体验**

的完整电影灯光连续体系。

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

每一次镜头切换必须回答：

```text
光源是否保持一致？

↓

光线方向是否一致？

↓

色温是否一致？

↓

人物是否仍处于同一光环境？

↓

AI 是否能够稳定生成？
```

连续性。

优先于局部美感。

---

# Lighting Continuity Philosophy

电影灯光连续性遵循：

```text
Story

↓

Scene

↓

Shot

↓

Lighting Continuity

↓

Audience
```

观众。

不能察觉灯光变化。

---

# Continuity Package

统一建立连续性数据。

```yaml
Lighting Continuity ID

Project ID

Sequence ID

Scene ID

Shot ID

Previous Shot

Next Shot

Validation Status
```

---

# Continuity Objectives

每一次灯光连续至少承担一种职责。

```yaml
Maintain Light Direction

Maintain Intensity

Maintain Color Temperature

Maintain Shadow

Maintain Reflection

Maintain Exposure

Maintain Atmosphere

Maintain Time

Maintain Identity

Audience Immersion
```

禁止：

无逻辑灯光变化。

---

# Continuity Hierarchy

统一控制层级。

```text
Story

↓

Scene

↓

Lighting

↓

Continuity

↓

Audience
```

灯光。

服从故事时间。

---

# Light Direction Continuity

统一光线方向。

```yaml
Front

Side

Back

Top

Bottom

Window Direction

Sun Direction

Practical Direction
```

方向。

保持一致。

---

# Intensity Continuity

统一亮度控制。

```yaml
Key Exposure

Fill Ratio

Highlight

Shadow Density

Ambient Level

Dynamic Range
```

亮度。

不得跳变。

---

# Color Temperature Continuity

统一色温。

```yaml
1800K

2700K

3200K

4500K

5600K

6500K

8000K
```

镜头之间。

保持逻辑一致。

---

# Shadow Continuity

统一阴影。

```yaml
Direction

Length

Density

Edge Softness

Pattern

Movement
```

阴影。

必须可信。

---

# Reflection Continuity

统一反射。

```yaml
Glass

Metal

Water

Floor

Wall

Skin
```

反射。

保持一致。

---

# Atmospheric Continuity

统一氛围。

```yaml
Fog

Smoke

Dust

Mist

Rain

Snow

Volumetric Light
```

环境光。

持续稳定。

---

# Time Continuity

统一时间变化。

```yaml
Morning

Day

Golden Hour

Sunset

Blue Hour

Night
```

时间推进。

必须合理。

---

# Character Lighting Continuity

统一人物灯光。

```yaml
Face Light

Eye Light

Hair Light

Skin Tone

Shadow Pattern

Rim Light
```

人物。

始终保持一致。

---

# Environment Continuity

统一环境灯光。

```yaml
Interior

Exterior

Natural

Artificial

Mixed Lighting

Transitional Space
```

空间。

形成统一视觉。

---

# Camera Coordination

摄影同步。

```yaml
Exposure

ISO

White Balance

HDR

Highlight Roll-off

Shadow Detail
```

摄影参数。

保持一致。

---

# AI Lighting Constraints

针对 AI 视频。

建立：

```yaml
Stable Light Direction

Stable Exposure

Stable Color Temperature

Stable Shadow

Stable Reflection

Stable Atmosphere
```

避免：

AI 灯光漂移。

---

# Workflow

```text
Scene Design

↓

Lighting Setup

↓

Continuity Check

↓

Correction

↓

Validation
```

连续性。

贯穿整部影片。

---

# Lighting Continuity Output

统一输出。

```yaml
Lighting Continuity Report

Exposure Match

Color Temperature Match

Shadow Match

Reflection Match

AI Constraint
```

供：

Lighting Validation。

Prompt Compiler。

Production Pipeline。

统一调用。

---

# Validation Rules

检查：

✓ 光源方向是否一致。

✓ 色温是否一致。

✓ 光比是否一致。

✓ 阴影是否一致。

✓ 环境光是否一致。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Lighting Validation。

---

# Lock Rules

锁定：

```yaml
Light Direction

Color Temperature

Exposure

Shadow Logic

Atmosphere Logic
```

允许：

后续模块补充：

```yaml
Validation

Platform Optimization
```

禁止修改：

灯光连续逻辑。

---

# Director Notes

自动生成。

```yaml
Continuity Score

Lighting Stability

Atmosphere Consistency

Narrative Continuity

Industrial Readiness

AI Stability
```

供导演、摄影指导（DoP）、灯光指导（Gaffer）、场记（Script Supervisor）、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影灯光连续性。

不是：

每一个镜头都不同。

而是：

所有镜头。

都像：

同一束光。

一直照耀着同一个故事。

因为：

电影中的光。

不仅照亮画面。

更连接时间。

连接空间。

连接观众。

Lighting Continuity Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影灯光连续性系统，为 Lighting Validation、Prompt Compiler 与 Production Pipeline 提供统一、稳定、具有电影工业标准的灯光连续性框架。
