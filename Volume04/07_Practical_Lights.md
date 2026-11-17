# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：07_Practical_Lights.md
# Priority：P4
# ============================================================

# Module

Practical Lights Engine

---

# Purpose

Practical Lights Engine（PLE）。

负责建立 Hollywood Director OS 中完整的 Practical Lighting（场景实景光源）系统。

Hollywood Director OS 认为：

真正优秀的电影灯光。

不仅来自摄影灯。

更来自：

**角色真正生活的世界。**

Practical Light 不是道具。

而是：

**故事的一部分。**

它既照亮空间。

也照亮人物。

更让观众相信：

这个世界是真实存在的。

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

每一个 Practical Light。

必须回答：

```text
为什么这里会有这盏灯？

↓

它属于谁？

↓

它是否影响剧情？

↓

人物是否会与它互动？

↓

观众是否相信它真实存在？
```

如果只是为了照亮画面。

禁止使用。

---

# Practical Lighting Package

统一建立数据。

```yaml
Practical ID

Scene ID

Shot ID

Fixture Type

Light Source

Lighting State

Interactive State

Narrative Purpose
```

---

# Practical Categories

统一分类。

```yaml
Table Lamp

Floor Lamp

Wall Lamp

Ceiling Light

Chandelier

Desk Lamp

Reading Lamp

TV Screen

Computer Monitor

Phone Screen

LED Strip

Neon Sign

Street Lamp

Traffic Light

Vehicle Headlight

Motorcycle Light

Police Beacon

Fireplace

Campfire

Torch

Candle

Lantern

Emergency Light

Exit Sign

Industrial Fixture
```

所有实景光源。

统一管理。

---

# Ownership Logic

每一个 Practical。

必须拥有：

```yaml
Owner

Environment

Architecture

Scene Function
```

例如：

```yaml
Bedroom

Table Lamp

Office

Monitor

Bar

Neon

Street

Street Lamp

Car

Headlight
```

不能凭空出现。

---

# Narrative Purpose

每一个 Practical。

至少承担一项职责。

```yaml
Reveal Character

Reveal Emotion

Reveal Space

Guide Attention

Trigger Event

Symbolism

Create Mood

Transition
```

---

# Interactive Lighting

允许角色改变灯光。

例如：

```yaml
Turn On Lamp

Turn Off Lamp

Open Refrigerator

Ignite Fire

Switch TV

Phone Unlock

Car Start

Open Door
```

所有互动。

同步更新：

Lighting State。

---

# Lighting State

统一状态。

```yaml
Off

Standby

On

Flicker

Broken

Emergency

Pulse
```

连续镜头。

必须继承。

---

# Brightness Profile

亮度等级。

```yaml
Very Low

Low

Medium

High

Extreme
```

亮度。

必须符合：

真实灯具。

---

# Color Profile

颜色统一。

```yaml
Warm

Neutral

Cool

RGB

Emergency Red

Police Blue

Fire Orange

Moon White
```

不得：

随机变化。

---

# Practical Hierarchy

建立优先级。

```text
Narrative Practical

↓

Character Practical

↓

Environmental Practical

↓

Decorative Practical
```

剧情相关。

优先级最高。

---

# Practical Interaction

记录人物关系。

```yaml
Look At

Touch

Carry

Turn On

Turn Off

Pass Through

Destroy

Repair
```

角色动作。

驱动灯光变化。

---

# Architecture Integration

灯具必须符合：

```yaml
Building Age

Architecture Style

Country

Region

Time Period
```

例如：

维多利亚时代。

不会出现：

现代 LED 灯带。

---

# Environmental Influence

环境影响灯具。

```yaml
Rain

Reflection

Fog

Glow

Dust

Light Beam

Smoke

Diffusion
```

真实融合。

---

# Reflection Strategy

Practical 自动产生：

```yaml
Glass Reflection

Floor Reflection

Metal Reflection

Water Reflection

Vehicle Reflection
```

形成：

空间真实感。

---

# Practical Rhythm

允许灯光节奏。

```yaml
Constant

Slow Flicker

Fast Flicker

Pulse

Random Failure

Heartbeat Pattern
```

仅用于：

剧情需要。

---

# AI Practical Constraints

针对 AI 视频。

增加：

```yaml
Stable Practical Position

Stable Brightness

Stable Color

Stable Reflection

Stable Flicker Pattern

Stable Interaction
```

避免：

AI 自动改变灯具。

---

# Practical Output

最终输出。

```yaml
Fixture Profile

Lighting State

Interaction Logic

Reflection Strategy

Narrative Purpose

Architecture Mapping

Environmental Response

AI Constraint
```

供：

AI Lighting Constraints。

Lighting Validation。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 灯具是否真实存在。

✓ 是否符合建筑。

✓ 是否符合年代。

✓ 是否符合剧情。

✓ 是否支持角色互动。

✓ 是否具有连续性。

✓ AI 是否稳定生成。

任何失败。

禁止进入：

AI Lighting Constraints。

---

# Lock Rules

锁定：

```yaml
Fixture Type

Lighting State

Interaction Logic

Narrative Purpose

Reflection Strategy
```

允许：

后续模块补充。

```yaml
Exposure Compensation

Lens Bloom

Lens Flare

Volumetric Scattering

HDR Highlight Roll-off
```

禁止修改：

Practical Light 逻辑。

---

# Director Notes

自动生成。

```yaml
Practical Authenticity

Interaction Quality

Narrative Contribution

Environmental Integration

Continuity Score

AI Practical Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的 Practical Light。

不是背景装饰。

而是角色生活的一部分。

角色打开一盏灯。

世界因此改变。

角色熄灭一支蜡烛。

故事因此进入黑暗。

Practical Lights Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的实景光源系统，为 AI Lighting Constraints、Lighting Validation、Color Pipeline 与 Prompt Compiler 提供真实、连续且具有叙事能力的灯光基础。

# End of File

# Next File

Volume04 / File：08_AI_Lighting_Constraints.md