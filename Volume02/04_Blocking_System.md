# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：04_Blocking_System.md
# Priority：P2
# ============================================================

# Module

Blocking System Engine

---

# Purpose

Blocking System Engine（BSE）。

负责建立真人电影的演员调度（Blocking）。

Hollywood Director OS 认为：

Blocking 不是走位。

Blocking 是：

**角色关系（Relationship）+ 戏剧目标（Objective）+ 空间设计（Space）+ 摄影协同（Camera）**。

演员每移动一步。

都必须推动故事。

---

# Position

```
Director Core

↓

Director Intent

↓

Shot Design

↓

Camera Language

↓

Blocking System

↓

180 Degree Rule

↓

Coverage
```

---

# Core Principle

每一次移动必须回答：

```
谁移动？

↓

为什么移动？

↓

移动到哪里？

↓

移动后关系改变了吗？

↓

摄影机为什么配合？
```

不能回答。

禁止移动。

---

# Blocking Package

每个 Segment 建立：

```yaml
Blocking ID

Scene ID

Segment ID

Shot ID

Primary Character

Supporting Character

Blocking Objective
```

---

# Blocking Objective

所有 Blocking 必须拥有唯一目标。

例如：

```yaml
Approach

Escape

Confront

Protect

Observe

Hide

Separate

Reconnect

Surround

Corner

Reveal

Delay
```

禁止：

无意义走位。

---

# Spatial Anchor

所有 Blocking 必须依赖：

Spatial Anchor。

例如：

```yaml
Door

Window

Desk

Sofa

Pillar

Vehicle

Stair

Wall
```

演员不能漂浮在空间。

必须始终依附空间锚点。

---

# Blocking Pattern

建立标准调度模型。

```yaml
Static

Linear

Cross

Circle

Triangle

Parallel

Opposition

Encirclement
```

例如：

双方谈判。

默认：

Opposition。

而不是随意站位。

---

# Character Distance

记录人物关系距离。

```yaml
Intimate

Personal

Social

Public
```

距离变化。

代表：

关系变化。

例如：

```
Social

↓

Personal

↓

Intimate
```

意味着信任增强。

---

# Facing Direction

记录角色朝向。

```yaml
North

South

East

West

Front

Back

Left

Right
```

所有镜头保持一致。

不得无故翻转。

---

# Movement Path

建立移动路径。

```yaml
Start

↓

Path

↓

Turning Point

↓

Destination
```

例如：

```text
Door

↓

Desk

↓

Window

```

摄影机自动继承。

---

# Blocking Beat

每一次 Blocking 拆分为：

```text
Prepare

↓

Move

↓

Stop

↓

Interact

↓

React
```

不是：

开始。

结束。

而是：

完整节拍。

---

# Interaction Zone

建立交互区域。

```yaml
Conversation Zone

Conflict Zone

Safe Zone

Danger Zone

Private Zone

Public Zone
```

角色进入不同区域。

自动影响：

表演。

摄影。

对白。

---

# Relationship Mapping

Blocking 自动更新：

```yaml
Character A

↓

Distance

↓

Character B

↓

Relationship State
```

例如：

双方靠近。

Relationship +10。

双方远离。

Relationship -10。

---

# Camera Coordination

Blocking 与摄影绑定。

记录：

```yaml
Camera Side

Actor Side

Movement Sync

Reveal Timing
```

摄影机不得破坏：

Blocking。

---

# Eye Line Mapping

建立：

视线关系。

```yaml
Look Target

Eye Height

Eye Direction

Eye Contact Duration
```

供：

180° Rule。

Performance Engine。

统一读取。

---

# Foreground / Background

建立层次。

```yaml
Foreground

Midground

Background
```

演员不能全部站同一平面。

必须建立空间深度。

---

# Entrance / Exit

所有角色。

必须拥有：

```yaml
Entry Point

Entry Timing

Exit Point

Exit Timing
```

禁止：

人物突然出现。

或突然消失。

---

# Blocking Rhythm

建立调度节奏。

```yaml
Still

↓

Move

↓

Pause

↓

Interaction

↓

Release
```

与：

Scene Rhythm。

同步。

---

# Environment Interaction

记录：

```yaml
Door

Open

↓

Chair

Move

↓

Curtain

Close

↓

Glass

Pick Up
```

Blocking 自动更新：

Scene State。

---

# Blocking Memory

建立状态继承。

```yaml
Previous Position

↓

Current Position

↓

Next Position
```

下一镜。

默认继承。

禁止：

人物瞬移。

---

# Crowd Blocking

多人场景建立：

```yaml
Leader

Followers

Background Actors

Flow Direction

Density

Attention Area
```

群众演员。

必须服务：

主角。

---

# Blocking Output

最终输出：

```yaml
Blocking Plan

Movement Path

Spatial Relationship

Interaction Zone

Relationship Update

Eye Line

Foreground Layer

Entry Exit Plan

Blocking Rhythm

Blocking Memory
```

供：

180 Degree Rule。

Coverage Engine。

Lighting Engine。

统一读取。

---

# Validation Rules

检查：

✓ Blocking Objective 是否唯一。

✓ 空间锚点是否建立。

✓ Movement 是否合理。

✓ Character Distance 是否连续。

✓ Eye Line 是否成立。

✓ Camera 是否同步。

✓ Relationship 是否更新。

✓ Entrance / Exit 是否完整。

✓ Blocking Memory 是否连续。

任何失败。

禁止进入：

180 Degree Rule。

---

# Lock Rules

锁定：

```yaml
Movement Path

Spatial Anchor

Relationship Distance

Eye Line

Blocking Memory
```

允许后续模块补充：

```yaml
摄影机轨迹

演员动作细节

光位调整

镜头覆盖方式
```

禁止修改：

Blocking 逻辑。

---

# Director Notes

系统自动生成：

```yaml
Blocking Complexity

Crossing Risk

Eye Line Risk

Camera Conflict

Performance Suggestion

Continuity Warning
```

供导演快速审核。

---

# Final Principle

Hollywood Director OS 中。

Blocking 不是让演员"站在哪"。

而是设计：

**角色关系如何变化。**

**观众注意力如何移动。**

**摄影机如何配合表演。**

优秀的 Blocking，不需要对白，也能让观众理解人物关系。

Blocking System Engine 输出的是一套符合好莱坞真人电影工业流程的演员调度系统，而不是简单的走位数据。

# End of File

# Next File

Volume02 / File：05_180_Degree_Rule.md
