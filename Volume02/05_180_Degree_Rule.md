# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：05_180_Degree_Rule.md
# Priority：P2
# ============================================================

# Module

180 Degree Rule Engine

---

# Purpose

180 Degree Rule Engine（180RE）。

负责维护真人电影中所有镜头的空间连续性（Spatial Continuity）。

Hollywood Director OS 将 180° 法则定义为：

**保证观众始终理解角色、空间、视线与运动方向的基础规则。**

它不仅是一条摄影规则。

更是：

导演、摄影、演员调度、剪辑共同遵守的空间语言。

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

Blocking

↓

180 Degree Rule

↓

Coverage

↓

Editing
```

---

# Core Principle

摄影机不能随意切换位置。

每一次跨越轴线。

必须回答：

```
为什么跨轴？

↓

观众是否会迷失方向？

↓

剧情是否允许？

↓

是否建立新的空间关系？
```

否则。

禁止跨轴。

---

# Axis Definition

系统自动建立：

```yaml
Axis ID

Scene ID

Segment ID

Primary Axis

Secondary Axis

Current Active Axis
```

所有镜头默认绑定：

Primary Axis。

---

# Axis Types

支持：

```yaml
Dialogue Axis

Movement Axis

Action Axis

Vehicle Axis

Crowd Axis

Object Axis

Environment Axis
```

每个 Segment。

只能有一个：

Primary Axis。

---

# Dialogue Axis

两人对白时。

自动建立：

```
Character A
────────────── Axis ──────────────
Character B
```

摄影机默认位于：

同一侧。

---

# Movement Axis

人物移动时。

建立：

```
Start

──────── Axis ────────>

End
```

摄影机保持：

运动方向一致。

---

# Camera Side

记录摄影机位置。

```yaml
Axis Left

Axis Right

Axis Center

Axis Transition
```

默认：

禁止：

Left ⇄ Right。

直接切换。

---

# Eye Line Continuity

自动维护：

```yaml
Character A

Look Right

↓

Character B

Look Left
```

禁止：

双方同时看向同一方向。

除非：

共同观察第三目标。

---

# Screen Direction

维护画面运动方向。

```yaml
Left → Right

Right → Left

Toward Camera

Away From Camera
```

整个 Scene。

默认保持一致。

---

# Crossing Conditions

允许跨轴。

必须满足以下之一。

```yaml
Character Moves

Camera Moves

Neutral Shot

Top Shot

Long Shot Reset

Motivated Transition
```

否则。

禁止跨越。

---

# Neutral Shot

允许使用：

Neutral Shot。

例如：

```yaml
Front Center

Top Down

Overhead

Drone

Symmetrical Shot
```

重新建立：

空间关系。

---

# Axis Reset

允许：

Scene 内建立新轴线。

例如：

角色：

转身。

移动。

进入新空间。

建立：

```yaml
Old Axis

↓

Transition Shot

↓

New Axis
```

旧轴线自动结束。

---

# Multiple Characters

多人场景。

建立：

Axis Network。

例如：

```text
A────────B

 \      /

   \  /

     C
```

系统自动选择：

Primary Axis。

其他：

Secondary Axis。

---

# Camera Transition

摄影机移动跨轴。

必须经过：

```yaml
Move Around

Orbit

Crane

Steadicam

Continuous Dolly
```

连续移动。

允许观众理解空间变化。

---

# Editing Protection

剪辑前自动检查：

```yaml
Previous Shot

↓

Axis Side

↓

Current Shot

↓

Axis Side
```

若：

直接反转。

输出：

Warning。

---

# Spatial Memory

建立：

空间记忆。

```yaml
Actor Position

Camera Position

Facing Direction

Movement Direction

Axis Side
```

所有镜头。

自动继承。

---

# Coverage Constraint

Coverage Engine。

必须遵守：

```yaml
OTS

Single

Two Shot

Insert

Reaction Shot
```

全部来自：

同一 Axis。

除非：

Reset。

---

# Action Scene Rules

动作戏允许：

动态轴线。

系统自动建立：

```yaml
Combat Axis

↓

Impact Axis

↓

Escape Axis
```

但必须：

逐步切换。

禁止：

随机翻转。

---

# Director Override

导演允许：

主动跨轴。

必须记录：

```yaml
Override Reason

Narrative Purpose

Audience Expectation

Recovery Shot
```

例如：

制造混乱。

心理崩溃。

梦境。

---

# 180 Rule Package

最终输出：

```yaml
Axis Map

Camera Side

Eye Line Map

Movement Direction

Crossing Record

Neutral Shot

Axis Reset

Spatial Memory
```

供：

Coverage。

Editing。

Continuity。

统一调用。

---

# Validation Rules

检查：

✓ Axis 是否建立。

✓ Camera Side 是否一致。

✓ Eye Line 是否正确。

✓ Movement Direction 是否连续。

✓ Crossing 是否合理。

✓ Reset 是否存在。

✓ Spatial Memory 是否同步。

✓ Coverage 是否遵守 Axis。

任何失败。

禁止进入：

Coverage Engine。

---

# Lock Rules

锁定：

```yaml
Primary Axis

Camera Side

Movement Direction

Eye Line

Spatial Memory
```

允许：

Coverage Engine 增加：

```yaml
镜头数量

覆盖方案

备用角度
```

禁止修改：

轴线逻辑。

---

# Director Notes

自动生成：

```yaml
Axis Warning

Eye Line Warning

Crossing Risk

Coverage Risk

Reset Recommendation
```

供导演快速审核。

---

# Final Principle

180 Degree Rule 不是限制摄影机。

而是保护观众。

Hollywood Director OS 始终认为：

观众必须始终知道：

**角色在哪里。**

**角色面对谁。**

**角色朝哪个方向移动。**

摄影机可以突破规则。

但导演必须知道：

为什么突破。

以及如何让观众重新建立空间认知。

180 Degree Rule Engine 的职责，就是维护整个电影的空间逻辑，使每一次镜头切换都清晰、可信且具有叙事价值。

# End of File

# Next File

Volume02 / File：06_Coverage_Strategy.md
