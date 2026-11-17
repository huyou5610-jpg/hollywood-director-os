# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume04
# Lighting Engine
# File：02_Key_Fill_Rim_System.md
# Priority：P4
# ============================================================

# Module

Key / Fill / Rim Lighting Engine

---

# Purpose

Key / Fill / Rim Lighting Engine（KFR）。

负责建立 Hollywood Director OS 的人物布光系统。

Hollywood Director OS 认为：

三点布光不是固定公式。

而是：

**塑造人物立体感、情绪与戏剧关系的光影结构。**

真正优秀的布光。

观众不会注意灯。

只会注意：

角色。

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

每一个人物布光。

必须回答：

```text
谁是主角？

↓

观众应该先看哪里？

↓

人物应该表现什么情绪？

↓

空间是否真实？

↓

光影是否符合导演意图？
```

---

# Lighting Package

统一输出。

```yaml
Lighting Setup ID

Shot ID

Key Light

Fill Light

Rim Light

Background Light

Eye Light

Lighting Ratio
```

---

# Lighting Hierarchy

建立控制流程。

```text
Story

↓

Character

↓

Emotion

↓

Lighting Structure

↓

Individual Lights
```

禁止：

先摆灯。

后决定人物。

---

# Key Light

主光承担：

```yaml
Reveal Face

Reveal Emotion

Primary Modeling

Narrative Direction
```

默认：

一个人物。

一个 Key。

---

# Key Direction

统一方向。

```yaml
Front 45°

Side 45°

Side 90°

Back 45°

Top

Window Direction
```

默认：

来源于真实光源。

---

# Key Quality

光质分类。

```yaml
Hard

Semi Hard

Soft

Very Soft
```

对应：

```yaml
Hard

Authority

Danger

Reality

Soft

Love

Memory

Comfort
```

---

# Fill Light

补光职责。

```yaml
Shadow Control

Skin Detail

Eye Detail

Contrast Balance
```

不是：

消灭阴影。

而是：

控制阴影。

---

# Fill Ratio

补光比例。

```yaml
None

Minimal

Balanced

High
```

例如：

```yaml
Film Noir

Almost None

Drama

Low Fill

Commercial

High Fill
```

---

# Rim Light

轮廓光职责。

```yaml
Separate Subject

Increase Depth

Create Elegance

Hero Effect
```

默认：

不抢主光。

---

# Rim Direction

允许：

```yaml
Back Left

Back Right

Top Back

Window Edge
```

必须：

具有来源。

---

# Hair Light

头发光。

仅用于：

```yaml
Dark Hair

Dark Background

Hero Close-up

Beauty
```

禁止：

所有镜头使用。

---

# Eye Light

眼神光。

职责：

```yaml
Catch Light

Life

Emotion

Attention
```

人物眼睛。

必须拥有生命力。

---

# Background Light

背景光承担：

```yaml
Depth

Space

Layer

Environment
```

禁止：

背景亮于人物。

---

# Lighting Ratio

统一比例。

```yaml
1:1

Flat

2:1

Natural

4:1

Drama

8:1

Noir

16:1

Extreme
```

根据剧情自动选择。

---

# Face Modeling

建立人物塑形。

```yaml
Strong

Natural

Soft

Beauty

Character
```

不同人物。

不同塑形。

---

# Multi Character Lighting

多人场景。

建立：

```yaml
Primary Character

Secondary Character

Background Character
```

光线优先：

主角。

---

# Emotional Mapping

情绪对应布光。

```yaml
Romance

Soft Key

Low Contrast

Crime

Hard Side Light

Political Drama

Natural Window

Thriller

Low Key

Action

Directional Hard Light
```

---

# Character Priority

人物权重。

```yaml
Lead Actor

★★★★★

Supporting

★★★★☆

Background

★★☆☆☆
```

灯光资源。

优先主角。

---

# Shadow Design

建立阴影策略。

```yaml
Open Shadow

Controlled Shadow

Deep Shadow

Split Shadow
```

阴影表达：

角色心理。

---

# Light Falloff

统一衰减。

```yaml
Gradual

Natural

Rapid
```

避免：

AI 产生硬切光区。

---

# Reflection Control

记录：

```yaml
Skin

Eyes

Glass

Metal

Water
```

控制：

高光反射。

---

# AI Lighting Constraints

针对 AI 视频。

增加：

```yaml
Stable Face Light

Stable Eye Light

Stable Rim

Stable Shadow Edge

No Flicker

No Light Jump
```

避免：

人物脸部闪烁。

---

# Lighting Output

最终输出。

```yaml
Key Profile

Fill Profile

Rim Profile

Background Light

Eye Light

Lighting Ratio

Shadow Strategy

AI Constraint
```

供：

Natural Lighting。

Cinematic Lighting。

统一调用。

---

# Validation Rules

检查：

✓ 主光是否明确。

✓ 补光是否合理。

✓ Rim 是否增强层次。

✓ Eye Light 是否自然。

✓ Lighting Ratio 是否符合剧情。

✓ 人物是否立体。

✓ AI 是否稳定。

任何失败。

禁止进入：

Natural Lighting。

---

# Lock Rules

锁定：

```yaml
Key Light

Fill Light

Rim Light

Lighting Ratio

Shadow Strategy
```

允许：

后续模块补充。

```yaml
灯具型号

功率

柔光附件

旗板

反光板

DMX 控制
```

禁止修改：

布光逻辑。

---

# Director Notes

自动生成。

```yaml
Face Modeling Score

Lighting Balance

Shadow Quality

Eye Light Score

Character Separation

AI Lighting Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的三点布光。

不是让人物变漂亮。

而是让人物变得可信。

Key Light 决定人物的存在。

Fill Light 决定人物的层次。

Rim Light 决定人物与世界的关系。

三者共同构成电影人物光影语言，并通过 AI Lighting Constraint 转换为 Seedance、Veo 等模型可稳定执行的灯光结构。

# End of File

# Next File

Volume04 / File：03_Natural_Lighting.md
