# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：08_Segment_Planner.md
# Priority：P1
# ============================================================

# Module

Segment Planner Engine

---

# Purpose

Segment Planner Engine（SPE）。

负责将已经完成导演规划的 Scene，组织成可以被 Director Engine 调度的 Shot Segment。

Segment 不是镜头。

Segment 也不是 Beat。

Segment 是：

**导演在同一戏剧目标下，可连续调度的一组镜头单元。**

它的职责不是切剧情。

而是组织镜头。

---

# Position

```
Script Parser

↓

Story Beat Engine

↓

Scene Breakdown

↓

Character Analysis

↓

Dialogue Breakdown

↓

Action Breakdown

↓

Emotion Breakdown

↓

Time Management

↓

Segment Planner Engine

↓

Director Engine
```

---

# Core Principle

Segment 必须满足：

```
One Story Beat

↓

One Dramatic Purpose

↓

One Visual Strategy

↓

One Emotional Direction

↓

One Editing Unit
```

任何 Segment。

不得跨越 Story Beat。

---

# Segment Hierarchy

```
Project

↓

Episode

↓

Sequence

↓

Scene

↓

Story Beat

↓

Segment

↓

Shot
```

Shot 属于 Segment。

Segment 服务 Beat。

---

# Segment Definition

每个 Segment 建立唯一编号。

```yaml
Segment ID

Scene ID

Beat ID

Segment Order

Segment Type

Director Objective

Estimated Duration
```

---

# Segment Type

自动分类：

```yaml
Opening Segment

Dialogue Segment

Performance Segment

Investigation Segment

Suspense Segment

Action Segment

Transition Segment

Reaction Segment

Ending Segment
```

允许组合。

但必须拥有：

Primary Segment。

---

# Segment Goal

每一个 Segment。

只能拥有一个导演目标。

例如：

```yaml
Introduce Character

Reveal Information

Increase Pressure

Build Suspense

Escalate Conflict

Release Emotion

Show Consequence

Prepare Transition
```

禁止：

多个导演目标混合。

---

# Segment Composition

每个 Segment 包含：

```yaml
Opening Shot

Supporting Shot

Reaction Shot

Insert Shot

Ending Shot
```

系统允许自动删减。

但必须存在：

Opening 与 Ending。

---

# Shot Allocation

自动建立：

```yaml
Shot 01

Purpose

↓

Shot 02

Purpose

↓

Shot 03

Purpose
```

每个 Shot。

只能承担一个信息点。

---

# Performance Focus

记录：

```yaml
Primary Performer

Performance Priority

Emotion Priority

Reaction Priority
```

摄影机围绕：

表演。

而不是动作。

---

# Camera Strategy

每个 Segment 建立统一摄影策略。

```yaml
Camera Language

Lens Style

Movement Style

Coverage Strategy

Editing Rhythm
```

例如：

```
Static

↓

Slow Push

↓

Handheld

↓

Locked-off
```

一个 Segment 内尽量保持一致。

---

# Blocking Strategy

建立：

演员调度方案。

```yaml
Entry

Movement

Interaction

Exit

Spatial Relationship
```

保证镜头之间：

空间连续。

---

# Continuity Memory

每个 Segment 自动记录：

```yaml
Character State

Emotion State

Action State

Camera State

Lighting State

Environment State
```

Ending State。

自动作为：

下一 Segment。

Start State。

---

# Segment Rhythm

建立节奏曲线。

```yaml
Opening

↓

Development

↓

Peak

↓

Release
```

导演可根据节奏调整：

镜头长度。

运镜速度。

对白密度。

---

# Editing Design

每个 Segment 输出：

```yaml
Cut Point

Transition Type

Reaction Buffer

Visual Bridge

Audio Bridge
```

保证后期：

自然衔接。

---

# Segment Output Package

最终输出：

```yaml
Segment Profile

Director Objective

Shot List

Performance Focus

Blocking Strategy

Camera Strategy

Continuity Memory

Editing Plan

Segment Rhythm
```

供 Director Engine 直接调用。

---

# Validation Rules

检查：

✓ Segment 是否只包含一个 Story Beat。

✓ Director Objective 是否唯一。

✓ Shot 是否职责明确。

✓ Camera Strategy 是否统一。

✓ Blocking 是否连续。

✓ Emotion 是否连续。

✓ Continuity Memory 是否完整。

✓ Editing Point 是否存在。

任何失败。

禁止进入 Director Engine。

---

# Lock Rules

锁定：

```yaml
Segment Goal

Story Beat

Shot Order

Camera Strategy

Continuity Memory
```

允许 Director Engine 补充：

```yaml
具体镜头设计

景别

焦段

运镜细节

导演备注
```

禁止修改：

Segment 结构。

---

# Director Preparation

Segment Planner 自动生成：

```yaml
Primary Shot Recommendation

Coverage Recommendation

Reaction Shot Priority

Insert Shot Suggestion

Editing Risk

Continuity Warning
```

Director Engine 可直接读取。

---

# Final Principle

Segment Planner 不负责设计镜头。

它负责建立导演真正工作的"调度单元"。

从这里开始，Hollywood Director OS 将不再面对剧本，而是面对一组已经完成故事、人物、情绪、动作、时间与连续性组织的导演级 Segment。

Director Engine 的全部分镜设计，都必须建立在 Segment Planner 输出的数据之上。

# End of File