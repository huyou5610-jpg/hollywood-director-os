# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：02_Scene_Breakdown.md
# Priority：P1
# ============================================================

# Module

Scene Breakdown Engine

---

# Purpose

Scene Breakdown Engine（SBD）。

负责将 Story Beat 组织成真正可以拍摄的 Scene（场景）。

Scene 不是地点。

也不是章节。

而是：

**具有统一戏剧目标、统一时间、统一空间、统一视觉逻辑的一组连续叙事单元。**

Scene 是导演工作的第一级单位。

Shot 是 Scene 的组成部分。

Beat 是 Scene 的叙事驱动。

---

# Position

```
Script Parser

↓

Story Beat Engine

↓

Scene Breakdown Engine

↓

Director Engine
```

---

# Core Principle

每一个 Scene 必须满足：

```
One Dramatic Goal

↓

One Time Span

↓

One Space

↓

One Emotional Arc

↓

One Visual Identity
```

任何一个条件被破坏。

重新拆分 Scene。

---

# Scene Definition

每个 Scene 建立唯一数据：

```yaml
Scene ID

Sequence ID

Episode ID

Scene Order

Scene Title

Scene Type

Scene Goal

Story Function

Estimated Duration

Beat Count
```

---

# Scene Type

自动识别：

```yaml
Opening Scene

Dialogue Scene

Action Scene

Investigation Scene

Suspense Scene

Romance Scene

Comedy Scene

Travel Scene

Transition Scene

Montage Scene

Climax Scene

Ending Scene
```

允许组合。

但必须有：

Primary Scene Type。

---

# Scene Goal

一个 Scene。

只能拥有一个主要目标。

例如：

```yaml
Introduce Character

Reveal Secret

Build Relationship

Increase Suspense

Deliver Information

Create Conflict

Resolve Conflict

Build Tension

Prepare Climax

End Story
```

禁止：

多个核心目标混杂。

---

# Scene Arc

每个 Scene 自动建立：

```text
Opening

↓

Development

↓

Turning Point

↓

Resolution

↓

Exit Point
```

Scene 不允许：

平铺直叙。

必须拥有变化。

---

# Scene Rhythm

建立：

Scene 节奏。

```yaml
Opening Pace

Middle Pace

Peak Pace

Ending Pace
```

例如：

```
Slow

↓

Medium

↓

Fast

↓

Slow
```

用于后续：

摄影节奏。

剪辑节奏。

对白节奏。

---

# Scene Emotion Arc

建立：

整场戏情绪变化。

例如：

```
Neutral

↓

Relaxed

↓

Suspicious

↓

Fear

↓

Despair
```

所有 Character Emotion。

必须服从：

Scene Emotion Arc。

---

# Scene Visual Identity

每个 Scene 建立唯一视觉标签。

包括：

```yaml
Visual Tone

Color Palette

Lighting Style

Contrast

Composition Style

Camera Language

Movement Style
```

一个 Scene 内默认保持统一。

除非剧情要求改变。

---

# Scene Timeline

记录：

```yaml
Scene Start Time

Scene End Time

Story Time

Real Time

Time Compression

Time Expansion
```

用于保证：

时间连续。

---

# Scene Space

建立：

空间数据。

```yaml
Location

Environment

Area

Entrances

Exits

Walkable Space

Obstacle

Height Difference

Important Objects
```

供 Blocking Engine 使用。

---

# Character Presence

记录：

```yaml
Main Character

Supporting Character

Background Character

Entry Point

Exit Point

Screen Time
```

每个角色。

必须记录：

进入。

离开。

停留状态。

---

# Scene State

建立：

Scene State Machine。

```yaml
Scene Start State

↓

Current State

↓

Scene End State
```

包括：

人物。

光照。

天气。

环境。

道具。

摄影机。

全部保存。

---

# Beat Mapping

每个 Beat。

绑定：

唯一 Scene。

```yaml
Beat 01

↓

Scene 01

Beat 02

↓

Scene 01

Beat 03

↓

Scene 01

Beat 04

↓

Scene 02
```

禁止：

一个 Beat 横跨多个 Scene。

---

# Scene Transition

自动分析：

Scene 如何进入下一 Scene。

```yaml
Cut

Match Cut

Graphic Match

Action Match

Dialogue Bridge

Sound Bridge

Fade

Dissolve

Time Cut

Location Cut
```

记录：

Transition Reason。

---

# Director Preparation

Scene 自动生成导演准备数据。

```yaml
Scene Objective

Audience Expectation

Key Performance

Visual Priority

Primary Conflict

Editing Focus
```

Director Engine 直接读取。

---

# Scene Package

最终输出：

```yaml
Scene ID

Scene Goal

Scene Arc

Scene Rhythm

Emotion Arc

Visual Identity

Timeline

Space

Characters

Beat List

Transition

Scene State
```

---

# Validation Rules

检查：

✓ Scene Goal 是否唯一。

✓ Scene 是否拥有完整 Arc。

✓ Beat 是否全部绑定。

✓ 时间是否连续。

✓ 空间是否连续。

✓ 情绪是否连续。

✓ Transition 是否存在。

✓ Visual Identity 是否统一。

任何一项失败。

禁止进入 Director Engine。

---

# Scene Lock

Validation 通过后。

锁定：

```yaml
Scene Goal

Scene Arc

Timeline

Space

Character List

Beat Mapping

Visual Identity

Scene State
```

后续 Engine。

只能读取。

不得修改。

---

# Scene Output

输出：

```
Scene Package

↓

Scene State Machine

↓

Director Preparation Data

↓

Scene Transition Map
```

---

# Final Principle

Scene Breakdown 的职责不是拆分文本。

而是建立导演真正工作的"场景单位"。

从这一刻开始，Hollywood Director OS 不再处理原始剧本，而是处理一组具有完整戏剧目标、视觉身份、空间关系和连续性状态的 Scene，为后续导演、摄影、演员调度和 Prompt 编译提供统一基础。

# End of File