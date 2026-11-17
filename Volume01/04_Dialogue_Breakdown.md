# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：04_Dialogue_Breakdown.md
# Priority：P1
# ============================================================

# Module

Dialogue Breakdown Engine

---

# Purpose

Dialogue Breakdown Engine（DBE）。

负责解析剧本中的所有对白。

对白不是文字。

而是：

**角色目标（Objective）+ 情绪（Emotion）+ 潜台词（Subtext）+ 节奏（Rhythm）+ 表演（Performance）**。

Hollywood Director OS 不把对白当成一句文本。

而是把对白当成：

**一次戏剧行为（Dramatic Action）**。

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

Dialogue Breakdown Engine

↓

Performance Engine
```

---

# Core Principle

每一句对白。

必须回答：

```
Who

谁说？

↓

Why

为什么说？

↓

To Whom

说给谁？

↓

Want

想得到什么？

↓

Result

结果是什么？
```

不能回答。

禁止进入下一模块。

---

# Dialogue Unit

每一句对白建立唯一 ID。

```yaml
Dialogue ID

Scene ID

Beat ID

Character ID

Dialogue Order
```

---

# Dialogue Package

每一句对白必须包含：

```yaml
Dialogue Text

Speaker

Target

Objective

Emotion

Subtext

Rhythm

Pause

Stress

Interruptions

Reaction

Ending State
```

---

# Dialogue Objective

对白必须有唯一目标。

例如：

```yaml
Persuade

Threaten

Comfort

Lie

Confess

Question

Test

Hide Truth

Challenge

Seduce

Reject

Negotiate

Command

Apologize
```

对白不是说话。

对白是在行动。

---

# Dialogue Emotion

建立对白情绪。

```yaml
Beginning Emotion

Peak Emotion

Ending Emotion
```

例如：

```
Calm

↓

Angry

↓

Controlled
```

---

# Subtext Engine

解析潜台词。

例如：

对白：

> "你今天回来得挺早。"

潜台词可能是：

```yaml
Concern

Suspicion

Jealousy

Relief

Testing
```

系统同时保存：

```
Literal Meaning

↓

Hidden Meaning

↓

Audience Meaning
```

---

# Dialogue Rhythm

建立节奏。

```yaml
Speech Speed

Sentence Length

Pause Density

Response Speed

Rhythm Curve
```

例如：

```
Slow

↓

Medium

↓

Fast

↓

Silence
```

---

# Pause Analysis

停顿不是空白。

停顿也是表演。

记录：

```yaml
Pause Position

Pause Duration

Pause Reason
```

Pause Reason：

```yaml
Thinking

Emotion

Pressure

Fear

Memory

Decision

Observation
```

---

# Stress Analysis

记录重音。

```yaml
Keyword

Stress Level

Purpose
```

例如：

> "我**没有**骗你。"

强调：

```
没有
```

改变语义。

---

# Breathing Analysis

对白绑定呼吸。

```yaml
Breathing Before

Breathing During

Breathing After
```

例如：

```
Short Breath

↓

Normal

↓

Heavy
```

供：

Performance Engine。

Audio Engine。

统一读取。

---

# Interruption Detection

识别：

```yaml
Self Interrupt

Character Interrupt

Environment Interrupt

Phone Interrupt

Explosion Interrupt

Emotion Interrupt
```

并建立：

对白中断点。

---

# Reaction Mapping

对白之后。

必须建立：

Reaction。

例如：

```yaml
Character A Speaks

↓

Character B

Eye Movement

↓

Micro Expression

↓

Breathing

↓

Action

↓

Dialogue
```

禁止：

对白没有反馈。

---

# Dialogue State

对白改变人物状态。

记录：

```yaml
Before Dialogue

↓

Dialogue

↓

After Dialogue
```

例如：

```
Trust 20

↓

Confession

↓

Trust 65
```

---

# Dialogue Beat

系统自动拆分：

Dialogue Beat。

例如：

```
Greeting

↓

Question

↓

Avoidance

↓

Pressure

↓

Confession

↓

Silence
```

Director Engine。

按 Beat 调度。

---

# Silence Analysis

沉默也是对白。

建立：

```yaml
Silence Type

Duration

Meaning

Audience Effect
```

例如：

```
Embarrassment

Shock

Power

Thinking

Fear

Love
```

---

# Multi-character Dialogue

多人对白。

建立：

Conversation Flow。

```text
A

↓

B

↓

A

↓

C

↓

B
```

自动分析：

谁主导。

谁防守。

谁逃避。

谁攻击。

---

# Dialogue Arc

每段对白建立完整弧线。

```text
Opening

↓

Build

↓

Conflict

↓

Turning Point

↓

Release

↓

Ending
```

禁止：

对白平铺直叙。

---

# Dialogue Influence

记录对白影响。

```yaml
Character Emotion

Relationship

Story

Conflict

Information

Scene Goal
```

所有变化。

自动更新：

Character State。

---

# Dialogue Package Output

最终输出：

```yaml
Dialogue Timeline

Dialogue Beat

Subtext Map

Stress Map

Pause Map

Breathing Map

Conversation Flow

Dialogue Arc

Dialogue State Change
```

供：

Performance Engine。

Audio Engine。

Director Engine。

统一读取。

---

# Validation Rules

检查：

✓ Speaker 是否唯一。

✓ Target 是否明确。

✓ Objective 是否存在。

✓ Emotion 是否完整。

✓ Subtext 是否建立。

✓ Pause 是否合理。

✓ Stress 是否存在。

✓ Dialogue 是否推动剧情。

✓ Reaction 是否建立。

✓ Ending State 是否更新。

任何一项失败。

禁止进入下一模块。

---

# Lock Rules

以下数据锁定：

```yaml
Dialogue Text

Speaker

Target

Objective
```

允许后续模块补充：

```yaml
Performance

Voice

Breathing

Camera Coverage

Audio Design
```

禁止修改对白本身。

---

# Final Principle

对白不是文字。

对白是角色达成目标的工具。

Hollywood Director OS 不拍一句台词。

而是拍一句台词背后的动机、情绪、潜台词、停顿、呼吸与人物关系变化。

因此，Dialogue Breakdown Engine 输出的不是对白文本，而是一套完整的对白表演数据。

# End of File