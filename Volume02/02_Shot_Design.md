# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：02_Shot_Design.md
# Priority：P2
# ============================================================

# Module

Shot Design Engine

---

# Purpose

Shot Design Engine（SDE）。

负责根据 Director Intent，将导演意图转换为真正可拍摄的镜头（Shot）。

Shot Design 不决定故事。

不决定人物。

不决定对白。

它唯一负责：

**设计镜头。**

镜头存在的唯一目的：

**让观众准确理解导演想表达的内容。**

---

# Position

```
Director Core

↓

Director Intent

↓

Shot Design Engine

↓

Camera Language

↓

Blocking

↓

Coverage

↓

Editing
```

---

# Core Principle

每一个镜头必须回答：

```
为什么存在？

↓

拍给谁看？

↓

表达什么？

↓

提供什么信息？

↓

结束后改变了什么？
```

如果回答不了。

删除镜头。

---

# Shot Hierarchy

```
Scene

↓

Story Beat

↓

Segment

↓

Shot
```

Shot 永远属于：

一个 Segment。

禁止跨 Segment。

---

# Shot Definition

每个镜头建立唯一数据。

```yaml
Shot ID

Scene ID

Segment ID

Shot Order

Shot Purpose

Shot Duration

Priority
```

---

# Shot Purpose

每个镜头只能承担一个核心任务。

例如：

```yaml
Introduce Character

Reveal Information

Show Reaction

Build Suspense

Increase Pressure

Establish Space

Show Relationship

Highlight Object

Deliver Emotion

Transition
```

禁止：

一个镜头承担多个核心信息。

---

# Shot Structure

每个镜头必须包含：

```yaml
Opening

↓

Development

↓

Peak

↓

Ending
```

即使只有2秒。

也必须拥有完整变化。

---

# Shot Information

定义：

镜头告诉观众什么。

```yaml
New Information

Repeated Information

Hidden Information

Emotional Information

Visual Information
```

禁止：

信息重复。

---

# Subject Priority

建立主体层级。

```yaml
Primary Subject

Secondary Subject

Background Subject

Environment
```

摄影机始终围绕：

Primary Subject。

---

# Emotional Focus

定义：

镜头主要表达：

```yaml
Performance

Dialogue

Action

Reaction

Environment

Silence
```

每个镜头。

只能有一个主要表达。

---

# Shot Timing

记录：

```yaml
Start Time

Peak Time

End Time

Hold Time
```

供：

剪辑。

摄影。

音乐同步。

---

# Shot Scale Hint

导演指定：

景别目标。

```yaml
Extreme Wide

Wide

Medium Wide

Medium

Medium Close

Close-up

Extreme Close-up
```

Camera Engine。

负责最终决定。

---

# Lens Hint

建立：

焦段建议。

```yaml
Ultra Wide

Wide

Normal

Portrait

Telephoto
```

这里只提供方向。

不是最终参数。

---

# Camera Motivation

记录：

摄影机为什么存在。

```yaml
Observe

Follow

Reveal

Witness

Hide

Investigate

Emotion

Relationship
```

禁止：

没有动机的镜头。

---

# Performance Priority

记录：

镜头优先捕捉：

```yaml
Eyes

Face

Body

Hands

Interaction

Movement
```

真人剧。

默认：

Eyes > Face > Body。

---

# Visual Composition Hint

建立：

构图目标。

```yaml
Center

Rule of Thirds

Symmetry

Negative Space

Foreground Frame

Depth Layer

Leading Lines
```

后续：

Camera Engine。

负责实现。

---

# Shot Rhythm

建立镜头节奏。

```yaml
Fast

Medium

Slow

Hold

Release
```

用于：

镜头长度。

摄影速度。

剪辑速度。

---

# Shot Transition

定义：

进入方式。

```yaml
Hard Cut

Match Cut

Reaction Cut

Insert

Push Transition

Audio Bridge
```

以及：

退出方式。

---

# Coverage Hint

自动判断：

是否需要：

```yaml
Master Shot

Two Shot

OTS

Single

Insert

Reaction

Cutaway
```

Coverage Engine。

继续扩展。

---

# Shot Dependency

记录：

当前镜头依赖：

```yaml
Previous Shot

Current Shot

Next Shot
```

保证：

摄影连续。

空间连续。

情绪连续。

---

# Shot Package

最终输出：

```yaml
Shot Profile

Shot Purpose

Information Target

Performance Focus

Visual Hint

Lens Hint

Composition Hint

Rhythm

Transition

Coverage Hint
```

供：

Camera Language Engine。

直接读取。

---

# Validation Rules

检查：

✓ Shot Purpose 是否唯一。

✓ Information 是否新增。

✓ Subject 是否明确。

✓ Camera Motivation 是否存在。

✓ Emotional Focus 是否明确。

✓ 节奏是否合理。

✓ Transition 是否存在。

✓ Director Intent 是否一致。

任何失败。

禁止进入：

Camera Language。

---

# Lock Rules

锁定：

```yaml
Shot Purpose

Performance Focus

Information Target

Camera Motivation

Coverage Hint
```

允许：

Camera Engine 补充：

```yaml
镜头高度

镜头角度

焦段

运动方式

摄影参数
```

禁止修改：

Shot Purpose。

---

# Director Notes

自动输出：

```yaml
Audience Attention

Performance Priority

Reaction Recommendation

Insert Recommendation

Editing Risk

Coverage Suggestion
```

---

# Final Principle

Shot Design Engine 不负责摄影技巧。

它负责建立导演真正需要的镜头逻辑。

镜头不是为了漂亮。

镜头是为了：

讲故事。

控制观众注意力。

表达角色情绪。

推动戏剧发展。

Hollywood Director OS 从这一层开始，正式进入电影镜头语言系统。

# End of File

# Next File

Volume02 / File：03_Camera_Language.md
