# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：07_Shot_Rhythm.md
# Priority：P2
# ============================================================

# Module

Shot Rhythm Engine

---

# Purpose

Shot Rhythm Engine（SRE）。

负责建立整部电影的镜头节奏（Shot Rhythm）。

Hollywood Director OS 认为：

节奏不是剪辑速度。

节奏也不是镜头长短。

节奏是：

**故事推进速度 + 演员表演节奏 + 摄影节奏 + 剪辑节奏 + 观众心理节奏。**

真正的电影节奏。

来自导演。

不是来自剪辑软件。

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

Coverage Strategy

↓

Shot Rhythm

↓

Lighting

↓

Editing
```

---

# Core Principle

每一个镜头都必须回答：

```
为什么现在切？

↓

为什么现在停？

↓

为什么继续保持？

↓

观众现在需要呼吸吗？

↓

观众现在需要紧张吗？
```

镜头节奏。

永远服务：

观众情绪。

---

# Rhythm Package

建立：

```yaml
Rhythm ID

Scene ID

Segment ID

Rhythm Type

Rhythm Curve

Narrative Pace

Emotion Pace
```

---

# Rhythm Hierarchy

系统建立四层节奏。

```text
Project Rhythm

↓

Sequence Rhythm

↓

Scene Rhythm

↓

Shot Rhythm
```

上层决定方向。

下层负责执行。

---

# Rhythm Types

统一分类。

```yaml
Static

Slow

Moderate

Fast

Explosive

Chaotic

Calm Recovery
```

每个 Scene。

必须拥有：

Primary Rhythm。

---

# Rhythm Curve

建立完整节奏曲线。

```text
Calm

↓

Build

↓

Pressure

↓

Peak

↓

Release

↓

Recovery
```

禁止：

全程一个速度。

---

# Shot Duration Logic

镜头长度。

必须根据戏剧目的决定。

例如：

```yaml
Emotion

Long

Dialogue

Medium

Action

Short

Suspense

Variable

Comedy

Precise
```

不是：

随机长短。

---

# Performance Rhythm

演员节奏优先。

建立：

```yaml
Breathing

Pause

Eye Contact

Reaction Delay

Speech Speed

Body Tempo
```

摄影必须跟随：

演员。

不是相反。

---

# Camera Rhythm

摄影运动节奏。

```yaml
Locked

↓

Slow Push

↓

Follow

↓

Fast Movement

↓

Hold
```

禁止：

摄影与演员节奏冲突。

---

# Editing Rhythm Hint

提供剪辑建议。

```yaml
Long Take

Invisible Cut

Reaction Cut

Rapid Cut

Cross Cut

Montage
```

只是导演建议。

不是最终剪辑。

---

# Emotional Rhythm

建立观众心理节奏。

```text
Observe

↓

Curiosity

↓

Suspense

↓

Anxiety

↓

Shock

↓

Silence

↓

Relief
```

所有镜头。

围绕此曲线安排。

---

# Silence Rhythm

系统认为：

沉默也是节奏。

记录：

```yaml
Silence Start

Silence Duration

Silence Purpose

Silence End
```

沉默不能空白。

必须承载信息。

---

# Dialogue Rhythm

对白节奏。

建立：

```yaml
Sentence Speed

Pause Length

Interruptions

Overlap

Reaction Gap
```

真人剧。

允许：

打断。

停顿。

沉默。

---

# Action Rhythm

动作节奏。

统一拆分：

```text
Preparation

↓

Execution

↓

Impact

↓

Recovery
```

不得：

全程高速。

---

# Rhythm Transition

记录：

```yaml
Previous Rhythm

Transition

Current Rhythm

Next Rhythm
```

例如：

```
Slow

↓

Acceleration

↓

Fast
```

转换必须自然。

---

# Audience Fatigue

系统自动检测：

```yaml
Fast Duration

Dialogue Density

Visual Density

Movement Density
```

如果：

持续高强度。

自动建议：

增加缓冲镜头。

---

# Rhythm Contrast

建立节奏反差。

例如：

```text
Long Silence

↓

Sudden Gunshot

↓

Fast Cut

↓

Still Frame
```

反差。

比速度更重要。

---

# Music Synchronization

输出：

```yaml
Beat Point

Emotion Peak

Silence Point

Transition Point
```

供音乐系统同步。

---

# Shot Rhythm Output

最终输出：

```yaml
Rhythm Curve

Performance Rhythm

Camera Rhythm

Dialogue Rhythm

Action Rhythm

Silence Rhythm

Transition Plan

Music Cue Point
```

供：

Lighting。

Editing。

Music。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ Rhythm Curve 是否完整。

✓ 节奏是否符合 Story Beat。

✓ 表演是否领先摄影。

✓ Camera 是否配合节奏。

✓ 沉默是否具有意义。

✓ 节奏是否拥有起伏。

✓ Audience Fatigue 是否合理。

✓ Emotion Curve 是否同步。

任何失败。

禁止进入：

Lighting Engine。

---

# Lock Rules

锁定：

```yaml
Rhythm Curve

Performance Rhythm

Dialogue Rhythm

Action Rhythm

Transition Plan
```

允许：

Editing Engine。

Music Engine。

补充执行方案。

禁止修改：

节奏逻辑。

---

# Director Notes

自动生成：

```yaml
Pacing Warning

Long Shot Suggestion

Cut Timing Suggestion

Silence Recommendation

Audience Fatigue Alert

Rhythm Balance
```

供导演调整。

---

# Final Principle

Hollywood Director OS 中。

节奏不是剪辑师创造的。

节奏诞生于导演。

镜头什么时候开始。

什么时候结束。

什么时候停留。

什么时候沉默。

共同构成电影真正的呼吸。

Shot Rhythm Engine 输出的不是镜头时长，而是一套完整、符合真人电影叙事规律的导演节奏系统。

# End of File

# Next File

Volume02 / File：08_Shot_Transition.md
