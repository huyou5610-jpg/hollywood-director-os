# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：01_Story_Beat.md
# Priority：P1
# ============================================================

# Module

Story Beat Engine

---

# Purpose

Story Beat Engine（SBE）。

负责将剧本转换成导演可以直接工作的 **Story Beat（故事节拍）**。

Story Beat 不是 Scene。

也不是 Shot。

而是：

**故事推进过程中，每一个具有明确戏剧目的的最小叙事单元。**

导演不是按段落拍戏。

而是按 Beat 拍戏。

因此。

所有后续模块。

统一读取：

Story Beat。

而不是原始剧本。

---

# Position

```
Script Parser

↓

Story Package

↓

Story Beat Engine

↓

Scene Breakdown

↓

Director Engine
```

---

# Core Principle

每一个 Beat。

必须回答五个问题：

```
Who

谁推动剧情？

↓

What

发生了什么？

↓

Why

为什么发生？

↓

Emotion

人物情绪发生什么变化？

↓

Story Value

故事因此改变了什么？
```

无法回答。

禁止建立 Beat。

---

# Beat Definition

一个 Beat 必须拥有：

```yaml
Beat ID

Scene ID

Beat Order

Story Function

Characters

Objective

Conflict

Emotion Shift

Information

Start State

End State
```

Beat ID 永久唯一。

禁止重复。

---

# Beat Hierarchy

```
Project

↓

Episode

↓

Sequence

↓

Scene

↓

Beat

↓

Shot
```

Shot 永远服务 Beat。

Beat 永远服务 Scene。

---

# Story Function

系统自动识别 Beat 的戏剧功能：

```
Character Introduction

Relationship

Setup

Foreshadowing

Question

Answer

Conflict

Escalation

Discovery

Decision

Reversal

Victory

Failure

Sacrifice

Climax

Resolution

Transition
```

至少选择一个。

---

# Beat Goal

每一个 Beat。

必须拥有唯一目标。

例如：

```yaml
让观众认识角色

建立危险感

暴露秘密

制造误会

推进感情

提升冲突

释放情绪

进入高潮
```

禁止：

多个核心目标混合。

---

# Beat Emotion

建立：

Emotion Curve。

例如：

```
Calm

↓

Suspicious

↓

Anxious

↓

Fear

↓

Relief
```

记录：

起点。

终点。

变化原因。

---

# Beat Conflict

记录：

冲突类型。

```
Character vs Character

Character vs Self

Character vs Environment

Character vs Society

Character vs Time

Character vs Unknown
```

每个 Beat 至少包含：

一种冲突。

或一次冲突缓解。

---

# Beat Information

记录：

本 Beat 向观众传递的信息。

例如：

```yaml
Reveal Killer

Reveal Relationship

Reveal Weakness

Reveal Secret

Reveal Goal

Reveal World Rule
```

禁止：

信息重复。

---

# Beat Transition

Beat 必须能够自然连接下一 Beat。

记录：

```yaml
Current Ending

↓

Next Beginning

↓

Transition Type
```

Transition Type：

```
Cut

Match Cut

Reaction

Action Match

Dialogue Bridge

Sound Bridge

Time Cut

Location Cut
```

---

# Beat Validation

每个 Beat 自动检查：

✓ 是否推动剧情。

✓ 是否改变人物状态。

✓ 是否改变观众信息量。

✓ 是否存在情绪变化。

✓ 是否拥有导演价值。

如果五项都没有变化。

删除 Beat。

---

# Beat Output

输出：

```yaml
Beat ID

Scene ID

Story Function

Goal

Conflict

Emotion

Information

Characters

Beginning

Ending

Transition
```

供：

Scene Breakdown。

Director Engine。

Performance Engine。

统一读取。

---

# Story Rhythm

系统自动分析：

Beat 节奏。

例如：

```
Slow

↓

Medium

↓

Fast

↓

Peak

↓

Release
```

避免：

连续多个高潮。

连续多个低谷。

保证节奏起伏。

---

# Director Notes

每个 Beat 自动生成导演备注：

```yaml
Director Intent

Audience Feeling

Visual Priority

Performance Focus

Editing Suggestion
```

注意：

这里只生成导演决策。

不生成镜头。

---

# Validation Rules

禁止：

一个 Beat 包含多个高潮。

禁止：

一个 Beat 同时跨多个 Scene。

禁止：

Beat 没有目标。

禁止：

Beat 没有结束状态。

禁止：

Beat 没有过渡方式。

---

# Final Output

Story Beat Engine 最终输出：

```yaml
Story Beat Package

↓

Beat Timeline

↓

Emotion Curve

↓

Conflict Progression

↓

Information Progression

↓

Transition Map
```

作为整个 Director Engine 的唯一故事输入。

---

# Final Principle

Hollywood Director OS 不直接根据剧本设计镜头。

而是先把剧本拆解成导演真正理解和控制的 Story Beat。

**导演控制的是 Beat。**

**摄影机拍摄的是 Beat。**

**演员表演的是 Beat。**

**Prompt 编译的也是 Beat。**

因此，Story Beat 是整个系统连接剧本与导演决策的核心桥梁。

# End of File