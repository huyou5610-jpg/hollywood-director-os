# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：06_Emotion_Breakdown.md
# Priority：P1
# ============================================================

# Module

Emotion Breakdown Engine

---

# Purpose

Emotion Breakdown Engine（EBE）。

负责建立整个 Hollywood Director OS 的情绪解析系统。

HDOS 不认为情绪只是：

快乐。

愤怒。

悲伤。

而认为情绪是：

**角色目标（Objective）+ 心理状态（Psychological State）+ 外部刺激（Trigger）+ 生理反应（Physical Response）+ 行为变化（Behavior）**。

情绪不是对白。

情绪也不是表情。

情绪是推动表演、摄影、镜头节奏和观众共鸣的核心驱动力。

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

Emotion Breakdown Engine

↓

Performance Engine
```

---

# Core Principle

每一次情绪变化。

必须回答：

```
Current Emotion

↓

Why Change

↓

Trigger

↓

Behavior Change

↓

Visible Expression

↓

End Emotion
```

禁止：

突然出现没有原因的情绪。

---

# Emotion Unit

每一次情绪变化建立唯一 Emotion ID。

```yaml
Emotion ID

Scene ID

Beat ID

Character ID

Emotion Order
```

---

# Emotion Package

每条情绪数据包含：

```yaml
Baseline Emotion

Current Emotion

Target Emotion

Emotion Trigger

Emotion Intensity

Emotion Duration

Visible Expression

Hidden Emotion

End State
```

---

# Baseline Emotion

每位角色建立默认情绪基线。

例如：

```yaml
Calm

Optimistic

Reserved

Aggressive

Melancholic

Confident
```

所有情绪变化。

必须基于 Baseline。

---

# Emotion Classification

系统统一采用情绪分类：

```yaml
Joy

Sadness

Fear

Anger

Disgust

Surprise

Love

Shame

Guilt

Hope

Despair

Relief

Curiosity

Suspicion

Determination
```

允许组合。

必须指定：

Primary Emotion。

---

# Emotion Trigger

记录情绪触发原因。

```yaml
Dialogue

Action

Memory

Environment

Relationship

Information

Physical Pain

Expectation

Failure

Success
```

没有 Trigger。

禁止建立情绪变化。

---

# Emotion Intensity

统一采用五级强度。

```yaml
Level 1

Subtle

----------------

Level 2

Noticeable

----------------

Level 3

Strong

----------------

Level 4

Extreme

----------------

Level 5

Breakdown
```

默认：

真实电影优先使用：

Level 1~3。

---

# Emotion Arc

每个角色建立情绪曲线。

```text
Neutral

↓

Concern

↓

Fear

↓

Resistance

↓

Acceptance
```

禁止：

情绪瞬间跳跃。

必须存在：

过渡过程。

---

# Visible Performance

情绪必须映射到演员可执行动作。

```yaml
Eye Movement

Facial Expression

Micro Expression

Breathing

Posture

Gesture

Voice

Movement Speed
```

例如：

Fear：

```
瞳孔放大

↓

呼吸变浅

↓

肩膀收紧

↓

说话变慢
```

---

# Hidden Emotion

记录角色真实情绪。

例如：

对白：

"我没事。"

Visible：

```yaml
Calm
```

Hidden：

```yaml
Fear
```

用于：

导演。

演员。

镜头设计。

---

# Emotion Transition

记录：

```yaml
Start Emotion

↓

Transition

↓

End Emotion
```

Transition 原因必须明确。

---

# Emotional Conflict

允许：

表里不一。

例如：

```yaml
Visible

Smile

Hidden

Anger
```

或：

```yaml
Visible

Calm

Hidden

Panic
```

供 Performance Engine 使用。

---

# Emotion Timeline

建立时间轴。

```yaml
Emotion Start

Emotion Peak

Emotion Recovery

Emotion End
```

供：

Camera。

Music。

Lighting。

同步。

---

# Emotion Influence

记录影响对象。

```yaml
Self

Relationship

Dialogue

Action

Decision

Story
```

例如：

恐惧。

导致：

拒绝开门。

改变剧情。

---

# Multi-character Emotion

多人同时存在时。

建立：

Emotion Network。

例如：

```text
A

Fear

↓

B

Anger

↓

C

Confusion
```

导演可根据冲突安排镜头优先级。

---

# Emotion Continuity

自动继承：

上一镜：

```yaml
Emotion

Intensity

Body State

Facial State

Voice State
```

默认延续。

除非：

Trigger 改变。

---

# Emotion Package Output

最终输出：

```yaml
Emotion Timeline

Emotion Arc

Emotion Trigger Map

Emotion Intensity Curve

Hidden Emotion

Visible Emotion

Emotion Continuity

Emotional Conflict
```

供：

Performance Engine

Camera Engine

Lighting Engine

Director Engine

统一读取。

---

# Validation Rules

检查：

✓ Baseline 是否建立。

✓ Trigger 是否存在。

✓ Emotion 是否合理。

✓ 强度是否连续。

✓ Hidden Emotion 是否明确。

✓ Visible Emotion 是否可表演。

✓ Emotion Arc 是否完整。

✓ End State 是否更新。

✓ Continuity 是否保持。

任何失败。

禁止进入 Performance Engine。

---

# Lock Rules

锁定：

```yaml
Emotion Trigger

Emotion Arc

Baseline Emotion
```

允许后续模块补充：

```yaml
Performance Detail

Camera Language

Lighting Support

Music Cue
```

禁止修改情绪逻辑。

---

# Director Notes

Emotion Engine 自动输出导演提示：

```yaml
Performance Priority

Reaction Shot Priority

Close-up Suggestion

Silence Recommendation

Camera Distance Recommendation
```

用于后续 Director Engine。

---

# Final Principle

Hollywood Director OS 不拍"情绪"。

而是拍：

**情绪产生的原因。**

**情绪在身体上的体现。**

**情绪如何改变角色行为。**

Emotion Breakdown Engine 输出的不是一个情绪标签，而是一套可供演员表演、摄影机捕捉、灯光强化、剪辑衔接的完整情绪系统。

# End of File