# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：05_Action_Breakdown.md
# Priority：P1
# ============================================================

# Module

Action Breakdown Engine

---

# Purpose

Action Breakdown Engine（ABE）。

负责解析剧本中的所有动作（Action）。

HDOS 不把动作理解为：

"人物做了一件事。"

而是理解为：

**角色目标 + 身体动力学 + 空间位移 + 环境交互 + 戏剧目的。**

动作不是动画关键帧。

动作是导演调度（Blocking）与演员表演（Performance）的共同基础。

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

Action Breakdown Engine

↓

Blocking Engine
```

---

# Core Principle

每一个动作必须回答：

```
Who

谁执行动作？

↓

Objective

为什么执行？

↓

Target

作用于谁或什么？

↓

Movement

身体如何运动？

↓

Result

动作结束后世界发生了什么变化？
```

---

# Action Unit

每个动作建立唯一 Action ID。

```yaml
Action ID

Scene ID

Beat ID

Character ID

Action Order
```

---

# Action Package

每个动作输出：

```yaml
Action Name

Action Type

Objective

Target

Start State

Action Beat

End State

Physics

Interaction

Environment Effect
```

---

# Action Classification

自动分类：

```yaml
Locomotion

Gesture

Interaction

Combat

Reaction

Facial Action

Object Manipulation

Environmental Action

Vehicle Action

Crowd Action
```

每个动作必须属于一个 Primary Type。

---

# Dramatic Objective

所有动作必须拥有戏剧目的。

例如：

```yaml
Approach

Escape

Attack

Defend

Observe

Hide

Search

Protect

Threaten

Comfort

Reveal

Delay
```

禁止为了"酷"而设计动作。

---

# Action Beat

一个动作拆解为多个 Action Beat。

标准结构：

```text
Preparation

↓

Initiation

↓

Execution

↓

Impact

↓

Recovery
```

例如：

挥拳：

```
握拳

↓

转肩

↓

挥拳

↓

命中

↓

收拳
```

后续 Camera Engine 依据 Beat 设计镜头。

---

# Motion State

动作必须记录状态。

```yaml
Body Position

Center of Gravity

Facing Direction

Velocity

Acceleration

Momentum

Balance
```

禁止只写：

"跑。"

必须记录：

**怎么跑。**

---

# Physics Model

建立真实物理。

```yaml
Weight Shift

Force Direction

Momentum

Gravity

Collision

Recovery
```

例如：

角色急停：

不是：

停止。

而是：

```
减速

↓

重心前移

↓

脚步调整

↓

恢复平衡
```

---

# Body Mechanics

拆分身体运动。

```yaml
Head

Eyes

Shoulders

Arms

Hands

Chest

Hip

Legs

Feet
```

每个动作自动分析：

哪些部位参与。

---

# Object Interaction

建立人与道具交互。

```yaml
Object

Interaction Type

Contact Point

Duration

State Change
```

例如：

```yaml
Object:

Door

Interaction:

Push

Result:

Door Open
```

道具状态同步更新。

---

# Character Interaction

建立人与人交互。

```yaml
Initiator

Receiver

Contact Type

Reaction

Relationship Effect
```

例如：

握手：

不仅记录：

动作。

同时更新：

Relationship。

---

# Environment Interaction

动作影响环境。

例如：

```yaml
Chair

Moved

↓

Glass

Broken

↓

Water

Splashed

↓

Curtain

Swinging
```

Scene State 自动更新。

---

# Action Rhythm

建立动作节奏。

```yaml
Preparation Speed

Execution Speed

Recovery Speed

Overall Rhythm
```

例如：

```
Slow

↓

Fast

↓

Hold

↓

Slow
```

---

# Action Energy

动作能量曲线。

```yaml
Energy Start

Energy Peak

Energy End
```

例如：

```
20

↓

90

↓

40
```

用于摄影机节奏同步。

---

# Reaction Chain

所有动作必须产生反馈。

```
Character A Pushes

↓

Character B Loses Balance

↓

Chair Falls

↓

Glass Breaks

↓

Silence
```

任何动作没有反馈。

视为不完整。

---

# Action Continuity

建立连续性数据。

```yaml
Previous Action

Current Action

Next Action

Carry State
```

例如：

上一镜：

举枪。

下一镜：

默认：

枪仍然举起。

禁止：

重新举枪。

---

# Action Timeline

记录：

```yaml
Action Start

Action Peak

Action End
```

用于：

剪辑。

摄影。

音乐。

音效同步。

---

# Action Package Output

最终输出：

```yaml
Action Timeline

Action Beat

Physics Model

Body Mechanics

Interaction Map

Environment Effect

Reaction Chain

Continuity State
```

供：

Blocking Engine

Performance Engine

Camera Engine

Continuity Engine

统一读取。

---

# Validation Rules

检查：

✓ Action Goal 是否存在。

✓ Action Beat 是否完整。

✓ Physics 是否合理。

✓ 重心是否连续。

✓ Interaction 是否建立。

✓ Reaction 是否存在。

✓ End State 是否更新。

✓ Continuity 是否保持。

✓ Environment 是否同步。

任何失败。

禁止进入 Blocking Engine。

---

# Lock Rules

以下数据锁定：

```yaml
Action Goal

Action Type

Target

Action Beat

Physics
```

允许后续模块补充：

```yaml
Performance Detail

Camera Coverage

Sound Design

Lighting Effect
```

禁止修改动作逻辑。

---

# Final Principle

Hollywood Director OS 中没有"简单动作"。

每一个动作都是：

人物目标的体现。

身体动力学的表现。

摄影机运动的依据。

连续性系统的状态源。

Action Breakdown Engine 输出的不是动作描述，而是一套完整、可拍摄、可连续、符合真人物理规律的 Action Data。

# End of File