# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume09
# Camera Engine
# File：03_Camera_Movement.md
# Priority：P9
# ============================================================

# Module

Camera Movement Engine

---

# Purpose

Camera Movement Engine（CME）。

负责建立 Hollywood Director OS 的电影摄影机运动系统（Cinema Camera Movement System）。

Hollywood Director OS 认为：

摄影机。

不仅决定：

看什么。

更决定：

**如何感受。**

摄影机运动。

不是炫技。

不是展示设备。

而是：

通过运动。

让观众参与故事。

Camera Movement 的职责。

就是建立：

**人物 → 情绪 → 摄影机运动 → 节奏 → 观众沉浸**

的完整电影摄影运动体系。

---

# Position

```text
Camera Theory

↓

Lens System

↓

Camera Movement

↓

Composition

↓

Blocking

↓

Visual Continuity

↓

Camera Validation
```

---

# Core Principle

每一次摄影机运动必须回答：

```text
为什么移动？

↓

为什么此刻移动？

↓

运动改变了什么？

↓

观众应该感受到什么？

↓

AI 是否能够稳定生成？
```

运动。

必须具有叙事目的。

---

# Camera Movement Philosophy

电影摄影运动遵循：

```text
Story

↓

Emotion

↓

Character

↓

Movement

↓

Audience
```

摄影机。

随着戏剧呼吸。

---

# Camera Movement Package

统一建立摄影运动数据。

```yaml
Movement ID

Project ID

Scene ID

Shot ID

Movement Type

Movement Speed

Movement Direction

Narrative Function

AI Constraint
```

---

# Movement Objectives

每一次运动至少承担一种职责。

```yaml
Reveal Character

Follow Action

Increase Emotion

Build Suspense

Clarify Space

Guide Audience

Transfer Power

Create Rhythm

Narrative Transition

Audience Immersion
```

禁止：

没有意义的运动。

---

# Movement Hierarchy

统一控制层级。

```text
Story

↓

Emotion

↓

Character

↓

Movement

↓

Audience
```

运动。

服从人物。

---

# Standard Movement Types

统一摄影运动类型。

```yaml
Static

Pan

Tilt

Dolly In

Dolly Out

Truck

Pedestal

Crane

Boom

Orbit

Arc

Tracking

Push In

Pull Back

Handheld

Steadicam

Drone

Zoom
```

统一工业命名。

---

# Narrative Mapping

不同运动。

承担不同叙事。

```yaml
Push In

Emotion

Pull Back

Isolation

Tracking

Journey

Orbit

Relationship

Crane Up

Liberation

Crane Down

Defeat

Static

Observation

Handheld

Chaos
```

运动。

表达故事。

---

# Camera Speed System

统一运动速度。

```yaml
Very Slow

Slow

Natural

Fast

Very Fast
```

速度。

影响情绪。

---

# Acceleration Curve

统一加速度。

```yaml
Ease In

Linear

Ease Out

Ease In Out

Sudden
```

避免：

机械运动。

---

# Movement Rhythm

统一运动节奏。

```yaml
Stillness

↓

Initiation

↓

Acceleration

↓

Peak

↓

Deceleration

↓

Hold
```

符合电影语言。

---

# Emotional Movement

摄影运动与情绪同步。

```yaml
Love

Slow Push

Fear

Handheld Shake

Hope

Ascending Crane

Sadness

Slow Pull Back

Power

Slow Dolly In

Chaos

Erratic Movement
```

运动。

强化情绪。

---

# Character Following

人物跟拍规则。

```yaml
Lead Follow

Side Follow

Rear Follow

Front Follow

Orbit Follow

Free Follow
```

摄影机。

跟随人物心理。

---

# Spatial Navigation

统一空间运动。

```yaml
Linear

Circular

Diagonal

Vertical

Curved

Multi-axis
```

建立空间连续性。

---

# Camera Stability Levels

统一稳定等级。

```yaml
Locked

Smooth

Organic

Dynamic

Chaotic
```

稳定程度。

服务叙事。

---

# Transition Movement

镜头转场运动。

```yaml
Match Move

Motivated Move

Whip Pan

Reveal Move

Pass Through

Hidden Cut
```

运动。

连接镜头。

---

# Movement & Lens Coordination

摄影运动与焦段同步。

```yaml
24mm Tracking

Environment

35mm Dolly

Narrative

50mm Push

Emotion

85mm Static

Performance

135mm Observation

Distance
```

镜头与运动。

共同叙事。

---

# AI Camera Movement Constraints

针对 AI 视频。

建立：

```yaml
Stable Motion Path

Stable Camera Height

Stable Speed Curve

Stable Character Tracking

Stable Horizon

Stable Motion Rhythm
```

避免：

AI 摄影机漂移。

---

# Workflow

```text
Story

↓

Emotion

↓

Movement Selection

↓

Speed Design

↓

Validation
```

运动。

来源于戏剧需求。

---

# Camera Movement Output

统一输出。

```yaml
Movement Library

Narrative Mapping

Speed Curve

Rhythm Design

Tracking Strategy

AI Constraint
```

供：

Composition。

Blocking。

Camera Validation。

统一调用。

---

# Validation Rules

检查：

✓ 是否具有叙事目的。

✓ 是否强化人物情绪。

✓ 是否符合摄影节奏。

✓ 是否保持空间连续。

✓ 是否避免无意义运动。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Composition。

---

# Lock Rules

锁定：

```yaml
Movement Logic

Motion Rhythm

Narrative Purpose

Tracking Rules

Speed Curves
```

允许：

后续模块补充：

```yaml
Composition

Blocking

Continuity
```

禁止修改：

摄影运动逻辑。

---

# Director Notes

自动生成。

```yaml
Movement Motivation

Narrative Quality

Rhythm Quality

Tracking Precision

Audience Engagement

AI Stability
```

供导演、摄影指导（DoP）、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的摄影机运动。

不是：

摄影机一直在移动。

而是：

它只在：

故事需要的时候。

开始移动。

因为：

每一次运动。

都是一次情绪变化。

每一次停止。

都是一次戏剧停顿。

摄影机。

不是在追逐人物。

而是在追逐：

**故事的情绪。**

Camera Movement Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影摄影机运动系统，为 Composition、Blocking、Visual Continuity、Camera Validation 与 Prompt Compiler 提供统一、稳定、具有电影级叙事节奏的摄影运动框架。
