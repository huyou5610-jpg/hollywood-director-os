# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：02_Camera_Movement.md
# Priority：P3
# ============================================================

# Module

Camera Movement Engine

---

# Purpose

Camera Movement Engine（CME）。

负责建立真人电影摄影机运动语言（Camera Movement Language）。

Hollywood Director OS 认为：

摄影机移动不是视觉特效。

摄影机移动代表：

**导演注意力的移动。**

真正优秀的运镜。

观众不会意识到摄影机在运动。

而会自然感受到：

故事正在推进。

---

# Position

```
Director Engine

↓

Cinematography Core

↓

Lens System

↓

Camera Movement

↓

Composition

↓

Depth

↓

Focus

↓

Exposure
```

---

# Core Principle

摄影机每一次运动。

必须回答：

```
为什么移动？

↓

是谁推动摄影机移动？

↓

运动是否增加叙事价值？

↓

停止的位置为什么在这里？

↓

观众获得了什么新的信息？
```

如果无法回答。

摄影机保持静止。

---

# Camera Movement Package

建立统一数据。

```yaml
Movement ID

Shot ID

Movement Type

Movement Motivation

Movement Direction

Movement Speed

Movement Duration

Movement Curve

Stop Position
```

---

# Movement Hierarchy

摄影机运动遵循：

```text
Story

↓

Emotion

↓

Performance

↓

Blocking

↓

Camera Movement
```

摄影机永远最后决定。

---

# Movement Categories

统一分类。

```yaml
Static

Pan

Tilt

Dolly

Truck

Pedestal

Crane

Push In

Pull Out

Orbit

Arc

Boom

Handheld

Steadicam

Gimbal

Whip Pan

Zoom

Drone

Virtual Camera
```

每个镜头。

只能存在一个：

Primary Movement。

---

# Narrative Motivation

所有运动必须拥有导演动机。

```yaml
Reveal

Follow

Observe

Discover

Investigate

Escape

Approach

Separation

Suspense

Emotion

Relationship

Scale
```

禁止：

"为了酷而运动。"

---

# Performance Driven

默认模式：

```yaml
Actor Moves

↓

Camera Responds
```

禁止：

```yaml
Camera Moves

↓

Actor 被迫配合
```

摄影机服务演员。

---

# Movement Direction

记录：

```yaml
Forward

Backward

Left

Right

Up

Down

Circular

Diagonal

Free
```

方向必须保持连续。

---

# Speed Profile

建立速度曲线。

```yaml
Very Slow

Slow

Medium

Fast

Explosive
```

以及：

```yaml
Ease In

Linear

Ease Out

Ease In Out
```

避免：

机械运动。

---

# Camera Energy

定义摄影能量。

```yaml
Calm

Neutral

Emotional

Aggressive

Chaotic
```

例如：

爱情戏：

Calm。

追逐戏：

Aggressive。

---

# Push In Logic

Push In 默认用于：

```yaml
Emotion Increase

Truth Reveal

Decision

Realization

Psychological Pressure
```

禁止：

频繁推镜。

---

# Pull Out Logic

Pull Out 默认用于：

```yaml
Isolation

Loss

Ending

Hopelessness

Reflection
```

---

# Pan & Tilt Logic

Pan：

用于：

```yaml
Follow

Reveal

Search

Relationship
```

Tilt：

用于：

```yaml
Scale

Power

Object

Height
```

禁止：

无目标摇镜。

---

# Dolly & Truck

Dolly：

改变：

观众距离。

Truck：

改变：

观察角度。

不得混用。

---

# Orbit / Arc

仅适用于：

```yaml
Romance

Psychological Conflict

Hero Moment

Revelation
```

必须拥有：

戏剧意义。

---

# Handheld Rules

允许：

```yaml
Chaos

Fear

War

Panic

Documentary

Subjective POV
```

普通对白。

默认禁止。

---

# Steadicam Rules

适用于：

```yaml
Following Character

Continuous Blocking

Long Take

Immersive Experience
```

保证：

稳定。

流畅。

---

# Zoom Rules

真人电影默认：

最低优先级。

仅用于：

```yaml
Documentary

Surveillance

Psychological Effect

1970s Style
```

现代剧情片。

优先：

Dolly。

而不是 Zoom。

---

# Camera Stop

摄影机停止。

必须拥有：

```yaml
Reason

Information Complete

Performance Peak

Composition Complete
```

不是：

运动结束。

而停止。

---

# Multi Movement

允许：

```text
Push In

↓

Pan

↓

Hold
```

最多：

三个连续动作。

禁止：

复杂炫技。

---

# AI Camera Constraints

AI 视频增加限制。

```yaml
Stable Velocity

Continuous Motion

No Random Shake

Predictable Curve

Consistent Direction

Frame Stability
```

避免：

生成漂移。

角色变形。

背景跳变。

---

# Movement Output

最终输出：

```yaml
Movement Profile

Movement Motivation

Movement Curve

Direction

Speed

Energy

Start Point

End Point

AI Motion Constraint
```

供：

Composition。

Focus。

Exposure。

统一调用。

---

# Validation Rules

检查：

✓ 是否拥有 Narrative Motivation。

✓ 是否符合 Director Intent。

✓ 是否跟随演员节奏。

✓ 是否符合 Blocking。

✓ 是否保持空间连续。

✓ 是否避免无意义运镜。

✓ AI 是否可稳定生成。

任何失败。

禁止进入：

Composition Engine。

---

# Lock Rules

锁定：

```yaml
Movement Type

Movement Motivation

Direction

Speed

Movement Curve
```

允许：

后续模块补充：

```yaml
Acceleration

Deceleration

Motion Blur

Camera Rig

Virtual Path
```

禁止修改：

摄影运动意图。

---

# Director Notes

自动生成：

```yaml
Movement Quality

Narrative Score

Performance Sync

Blocking Conflict

AI Stability Score

Movement Suggestion
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

摄影机不会自己移动。

真正推动摄影机的。

永远是：

**角色。**

**故事。**

**情绪。**

摄影机只是观众意识的延伸。

每一次推进。

代表观众更加靠近人物。

每一次后退。

代表观众重新审视世界。

Camera Movement Engine 输出的是一套符合好莱坞真人电影工业标准、兼容 AI 视频生成的摄影机运动语言系统，而不是简单的运镜参数。

# End of File

# Next File

Volume03 / File：03_Composition_System.md

```