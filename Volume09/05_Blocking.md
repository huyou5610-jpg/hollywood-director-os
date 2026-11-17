# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume09
# Camera Engine
# File：05_Blocking.md
# Priority：P9
# ============================================================

# Module

Blocking Engine

---

# Purpose

Blocking Engine（BE）。

负责建立 Hollywood Director OS 的电影调度系统（Cinema Blocking System）。

Hollywood Director OS 认为：

摄影机决定：

看哪里。

构图决定：

如何组织画面。

而：

**调度（Blocking）决定故事如何发生。**

电影中的人物。

不是站在画面里。

而是：

在空间中行动。

在关系中移动。

在冲突中改变。

Blocking 的职责。

就是建立：

**人物 → 空间 → 运动 → 摄影机 → 戏剧关系**

的完整电影调度体系。

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

每一次调度必须回答：

```text
角色为什么站在这里？

↓

为什么此刻移动？

↓

移动改变了什么？

↓

人物关系发生了什么变化？

↓

AI 是否能够稳定生成？
```

调度。

必须推动戏剧。

---

# Blocking Philosophy

电影调度遵循：

```text
Story

↓

Character

↓

Relationship

↓

Space

↓

Movement

↓

Audience
```

人物移动。

源于故事。

---

# Blocking Package

统一建立调度数据。

```yaml
Blocking ID

Project ID

Scene ID

Shot ID

Character Position

Movement Path

Interaction Point

Camera Relation

Narrative Function
```

---

# Blocking Objectives

每一次调度至少承担一种职责。

```yaml
Advance Story

Reveal Character

Build Relationship

Transfer Power

Clarify Space

Increase Tension

Support Camera

Guide Audience

Support Performance

Narrative Focus
```

禁止：

没有戏剧目的的移动。

---

# Blocking Hierarchy

统一控制层级。

```text
Story

↓

Relationship

↓

Character

↓

Blocking

↓

Audience
```

调度。

服从人物关系。

---

# Character Positioning

统一人物站位。

```yaml
Center

Leader

Foreground

Focus

Background

Observation

Side

Conflict

Diagonal

Dynamic

Circle

Negotiation
```

站位。

表达身份。

---

# Movement Path

统一运动路径。

```yaml
Straight

Curved

Circular

Diagonal

Cross

Approach

Retreat

Random
```

路径。

体现心理。

---

# Relationship Distance

统一人物距离。

```yaml
Intimate

Personal

Social

Public

Separated

Opposed
```

距离。

体现关系变化。

---

# Power Blocking

统一权力调度。

```yaml
Higher Position

Dominance

Lower Position

Submission

Forward

Initiative

Backward

Retreat

Center

Authority

Edge

Isolation
```

空间。

体现权力。

---

# Entrance Strategy

统一入场设计。

```yaml
Visible Entry

Hidden Entry

Reveal Entry

Delayed Entry

Background Entry

Foreground Entry
```

出场。

建立戏剧期待。

---

# Exit Strategy

统一退场设计。

```yaml
Frame Exit

Fade Exit

Back Exit

Foreground Exit

Hidden Exit

Motivated Exit
```

退场。

结束戏剧动作。

---

# Interaction Blocking

人物互动调度。

```yaml
Face To Face

Side By Side

Cross Movement

Passing

Circling

Confrontation

Support

Protection
```

互动。

改变关系。

---

# Multi-character Blocking

多人调度。

统一设计。

```yaml
Leader

Followers

Groups

Opposition

Triangle

Circle

Layered
```

多人场景。

保持清晰。

---

# Environmental Blocking

环境参与调度。

```yaml
Door

Window

Table

Chair

Wall

Vehicle

Architecture

Landscape
```

空间。

参与表演。

---

# Camera Coordination

摄影与调度同步。

```yaml
Static Camera

Character Movement

Moving Camera

Shared Movement

Locked Composition

Dynamic Blocking

Tracking

Motivated Follow
```

摄影机。

服从调度节奏。

---

# Performance Coordination

调度与表演同步。

```yaml
Movement

Dialogue

Eye Contact

Gesture

Pause

Reaction
```

调度。

强化表演。

---

# Rhythm Design

统一调度节奏。

```yaml
Still

↓

Movement

↓

Interaction

↓

Conflict

↓

Resolution
```

空间。

具有节奏。

---

# AI Blocking Constraints

针对 AI 视频。

建立：

```yaml
Stable Character Position

Stable Movement Path

Stable Distance

Stable Orientation

Stable Interaction Timing

Stable Spatial Logic
```

避免：

AI 人物位置漂移。

---

# Workflow

```text
Story

↓

Relationship

↓

Blocking Design

↓

Camera Coordination

↓

Validation
```

调度。

来源于人物关系。

---

# Blocking Output

统一输出。

```yaml
Blocking Map

Movement Path

Relationship Distance

Power Layout

Camera Coordination

AI Constraint
```

供：

Visual Continuity。

Camera Validation。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 是否推动剧情。

✓ 是否强化人物关系。

✓ 是否符合空间逻辑。

✓ 是否支持摄影设计。

✓ 是否强化表演。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Visual Continuity。

---

# Lock Rules

锁定：

```yaml
Blocking Logic

Movement Path

Relationship Distance

Power Layout

Spatial Rules
```

允许：

后续模块补充：

```yaml
Continuity

Editing

AI Optimization
```

禁止修改：

人物调度逻辑。

---

# Director Notes

自动生成。

```yaml
Blocking Quality

Relationship Clarity

Spatial Readability

Performance Support

Narrative Strength

AI Stability
```

供导演、摄影指导（DoP）、副导演、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影调度。

不是：

演员走到哪里。

而是：

每一步移动。

都改变了：

人物关系。

空间权力。

戏剧张力。

观众情绪。

因为：

电影里的移动。

从来不是走位。

而是：

**故事正在流动。**

Blocking Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影调度系统，为 Visual Continuity、Camera Validation 与 Prompt Compiler 提供统一、稳定、具有电影级空间叙事能力的人物调度框架。
