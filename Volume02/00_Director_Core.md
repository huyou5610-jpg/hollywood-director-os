# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：00_Director_Core.md
# Priority：P2
# ============================================================

# Module

Director Core Engine

---

# Purpose

Director Core Engine（DCE）。

是整个 Hollywood Director OS 的核心。

从这一模块开始。

系统正式停止：

分析剧本。

开始：

导演电影。

Director Engine 不负责理解故事。

Story Engine 已完成。

Director Engine 的职责只有一个：

**把已经验证完成的故事，拍成一部电影。**

---

# Position

```
Validated Story Package

↓

Director Core Engine

↓

Director Intent

↓

Shot Design

↓

Camera Language

↓

Blocking

↓

Coverage

↓

Prompt Compiler
```

---

# Director Philosophy

HDOS 永远遵循：

导演思维。

而不是：

Prompt 思维。

任何镜头。

任何摄影。

任何灯光。

任何演员调度。

必须回答：

> 为什么导演要这样拍？

而不是：

> AI 能不能这样生成？

---

# Director Decision Hierarchy

导演所有决策。

必须遵循固定顺序。

```
Story

↓

Story Beat

↓

Scene Goal

↓

Director Intent

↓

Audience Emotion

↓

Actor Performance

↓

Blocking

↓

Camera

↓

Composition

↓

Lighting

↓

Editing

↓

Prompt
```

禁止跳级。

禁止逆序。

---

# Director Responsibility

Director Engine 唯一负责：

```yaml
Audience Emotion

Storytelling

Performance

Visual Rhythm

Shot Logic

Editing Logic

Visual Continuity
```

以下内容禁止修改：

```yaml
Story

Dialogue

Character Setting

Story Beat

Scene Goal
```

---

# Director Inputs

Director Engine 统一读取：

```yaml
Validated Story Package

Scene Package

Character Database

Dialogue Package

Action Package

Emotion Package

Timeline Package

Segment Package
```

不得读取：

用户原始文本。

---

# Director Outputs

统一输出：

```yaml
Director Intent

Scene Objective

Shot Strategy

Blocking Strategy

Camera Strategy

Coverage Strategy

Editing Strategy
```

---

# Director Thinking Loop

每一个 Scene。

导演必须循环思考：

```
这一场戏真正讲什么？

↓

观众应该感受到什么？

↓

谁是主角？

↓

谁推动剧情？

↓

谁改变局势？

↓

什么时候切镜头？

↓

什么时候保持镜头？

↓

什么时候保持沉默？

↓

什么时候结束？
```

全部完成。

才能设计镜头。

---

# Scene Objective

每个 Scene。

必须建立唯一导演目标。

例如：

```yaml
Increase Pressure

Reveal Truth

Create Romance

Build Mystery

Create Isolation

Build Sympathy

Escalate Conflict

Release Emotion
```

所有镜头。

全部服务：

Scene Objective。

---

# Audience Emotion

导演必须定义：

```yaml
Audience Beginning Emotion

Audience Peak Emotion

Audience Ending Emotion
```

例如：

```
Curiosity

↓

Suspense

↓

Shock
```

摄影。

剪辑。

音乐。

全部围绕此设计。

---

# Visual Priority

导演指定：

```yaml
Primary Subject

Secondary Subject

Background

Visual Focus

Eye Path
```

保证：

观众永远知道：

该看哪里。

---

# Performance Priority

建立：

```yaml
Primary Actor

Primary Emotion

Reaction Priority

Silence Priority

Micro Expression Priority
```

真人剧：

演员永远优先于摄影机。

---

# Camera Motivation

摄影机不能随便移动。

每次移动必须拥有：

```yaml
Narrative Reason

Performance Reason

Information Reason

Emotion Reason
```

禁止：

无意义运镜。

---

# Editing Awareness

导演设计镜头时。

必须提前思考：

```yaml
Where To Cut

Why Cut

When Hold

Reaction Timing

Insert Timing

Transition Timing
```

镜头必须：

可剪辑。

---

# Director State Machine

每个 Scene。

维护导演状态。

```yaml
Scene Objective

↓

Current Dramatic Focus

↓

Audience Emotion

↓

Visual Strategy

↓

Ending State
```

下一 Scene。

自动继承。

---

# Director Package

最终输出：

```yaml
Director Goal

Audience Emotion

Scene Objective

Performance Priority

Visual Priority

Camera Motivation

Editing Awareness

Director Notes
```

供：

Director Intent Engine。

直接读取。

---

# Validation Rules

检查：

✓ 是否存在唯一 Scene Objective。

✓ 是否存在 Audience Emotion。

✓ 是否明确主角。

✓ 是否明确视觉中心。

✓ 是否存在 Camera Motivation。

✓ 是否存在 Editing Logic。

✓ 是否符合 Story Beat。

✓ 是否符合 Scene Goal。

任何失败。

禁止进入：

Director Intent。

---

# Lock Rules

锁定：

```yaml
Scene Objective

Audience Emotion

Visual Priority

Performance Priority

Camera Motivation
```

后续模块。

只能扩展。

不得修改。

---

# Final Principle

Hollywood Director OS 的 Director Core。

不是决定镜头怎么拍。

而是决定：

**为什么拍。**

只有导演目标明确。

镜头语言才有意义。

只有观众情绪明确。

摄影、表演、灯光、剪辑才能形成统一表达。

Director Core 是整个 Director Engine 的唯一决策源。

# End of File