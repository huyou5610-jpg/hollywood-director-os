# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：01_Light_Motivation.md
# Priority：P4
# ============================================================

# Module

Light Motivation Engine

---

# Purpose

Light Motivation Engine（LME）。

负责建立 Hollywood Director OS 中所有电影灯光的**动机系统（Motivated Lighting）**。

Hollywood Director OS 认为：

电影里的每一道光。

都必须拥有：

**存在理由。**

观众不一定知道灯为什么在那里。

但必须相信：

它本来就应该在那里。

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
```

---

# Core Principle

任何灯光。

必须回答：

```text
光从哪里来？

↓

为什么存在？

↓

角色为什么会被照亮？

↓

观众为什么相信？

↓

光是否推动剧情？
```

如果不能回答。

禁止使用。

---

# Motivation Hierarchy

建立灯光来源层级。

```text
Story

↓

Environment

↓

Architecture

↓

Practical Source

↓

Cinematic Enhancement

↓

Exposure Compensation
```

灯光不能反向设计。

---

# Motivation Package

统一输出。

```yaml
Motivation ID

Scene ID

Shot ID

Primary Source

Secondary Source

Hidden Source

Light Direction

Narrative Purpose
```

---

# Primary Light Source

真实来源。

```yaml
Sun

Sky

Window

Door

Lamp

Fire

TV

Phone

Monitor

Neon

Vehicle

Moon

Street Light

Practical Fixture
```

每个镜头。

必须存在：

Primary Source。

---

# Secondary Source

辅助来源。

```yaml
Bounce

Wall Reflection

Ground Reflection

Practical Fill

Ambient

Sky Fill

Indirect Window
```

不能喧宾夺主。

---

# Hidden Source

电影允许：

隐藏光源。

例如：

```yaml
Invisible Soft Light

Invisible Eye Light

Invisible Rim

Invisible Bounce

Invisible Fill
```

原则：

观众不能察觉。

---

# Motivation Categories

统一分类。

```yaml
Natural

Architectural

Practical

Environmental

Narrative

Psychological

Symbolic
```

默认：

Natural 优先。

---

# Narrative Motivation

灯光承担剧情目的。

```yaml
Reveal

Hide

Separate

Guide

Emphasize

Threaten

Comfort

Transform
```

每盏灯。

必须至少承担：

一种功能。

---

# Emotional Mapping

不同情绪。

对应不同光源。

```yaml
Hope

Morning Sun

Fear

Single Practical

Love

Warm Window

Loneliness

Cold Sky

Mystery

Partial Shadow

Power

Hard Top Light

Memory

Soft Diffused Light
```

禁止：

情绪与灯光冲突。

---

# Architectural Logic

建筑决定光。

例如：

```yaml
Window Direction

Ceiling Height

Door Position

Corridor

Glass

Curtain

Concrete

Wood
```

建筑结构。

优先于摄影需求。

---

# Time Logic

光必须符合时间。

```yaml
Morning

Noon

Afternoon

Golden Hour

Blue Hour

Night

Midnight
```

禁止：

午夜太阳光。

---

# Weather Logic

天气控制光质。

```yaml
Sunny

Hard Light

Cloudy

Soft Light

Rain

Low Contrast

Fog

Atmospheric Diffusion

Snow

High Reflection
```

不得违背天气。

---

# Character Motivation

角色行为。

影响灯光。

例如：

```yaml
Open Curtain

↓

Light Change

Turn On Lamp

↓

Practical Source

Open Door

↓

Exterior Spill

Phone Screen

↓

Face Fill
```

角色推动光线。

---

# Camera Motivation

摄影机位置。

决定：

哪些光源可见。

```yaml
Visible Source

Hidden Source

Off Screen Source
```

保证：

摄影真实。

---

# Light Direction Logic

统一方向。

```yaml
Front

Side

Back

Top

Bottom

Diagonal
```

方向。

必须符合：

真实来源。

---

# Intensity Motivation

亮度来源。

```yaml
Weak

Natural

Strong

Extreme
```

不是：

摄影师决定。

而是：

环境决定。

---

# Practical Lighting Rules

允许：

```yaml
Table Lamp

Wall Lamp

Street Lamp

TV

Computer

Fireplace

Car Headlight

Emergency Light
```

优先：

真实存在。

---

# Psychological Lighting

特殊情况下。

允许：

心理灯光。

例如：

```yaml
Nightmare

Dream

Memory

Hallucination

Religious Vision
```

必须：

Director Approval。

---

# AI Motivation Constraints

AI 视频增加：

```yaml
Stable Source

Stable Direction

Stable Shadow

Stable Reflection

Stable Practical
```

避免：

AI 自动改变光源。

---

# Motivation Workflow

```text
Story

↓

Environment

↓

Architecture

↓

Primary Source

↓

Secondary Source

↓

Narrative Enhancement

↓

Validation
```

禁止：

反向设计。

---

# Motivation Output

统一输出。

```yaml
Primary Source

Secondary Source

Light Direction

Motivation Type

Narrative Purpose

Architectural Logic

Environmental Logic

AI Constraint
```

供：

Key / Fill / Rim。

Natural Lighting。

统一调用。

---

# Validation Rules

检查：

✓ 是否拥有真实来源。

✓ 是否符合建筑逻辑。

✓ 是否符合时间。

✓ 是否符合天气。

✓ 是否符合角色行为。

✓ 是否符合导演意图。

✓ AI 是否可稳定生成。

任何失败。

禁止进入：

Key / Fill / Rim System。

---

# Lock Rules

锁定：

```yaml
Primary Source

Secondary Source

Direction

Motivation

Narrative Purpose
```

允许：

Lighting Engine。

补充：

```yaml
Light Size

Diffusion

Intensity

Lighting Ratio

Rig Position
```

禁止修改：

灯光来源。

---

# Director Notes

自动生成：

```yaml
Motivation Score

Source Visibility

Architectural Accuracy

Narrative Support

Realism Score

AI Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影灯光。

不会让观众觉得：

"这里打了一盏灯。"

而会让观众相信：

**太阳本来就会照进来。**

**那盏台灯本来就在亮着。**

**火焰本来就会照亮人物。**

Light Motivation Engine 的职责。

就是确保所有灯光都拥有真实可信的存在理由，并将真实世界的光照逻辑转换为 AI 能稳定理解和持续生成的电影灯光语言。

# End of File

# Next File

Volume04 / File：02_Key_Fill_Rim_System.md