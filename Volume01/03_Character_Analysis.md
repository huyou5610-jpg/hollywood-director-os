# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：03_Character_Analysis.md
# Priority：P1
# ============================================================

# Module

Character Analysis Engine

---

# Purpose

Character Analysis Engine（CAE）。

负责建立整个项目唯一可信的角色数据库（Character Database）。

HDOS 不把角色理解为：

一个名字。

一个外貌。

而是理解为：

**一个持续变化、持续成长、持续影响剧情的生命体。**

所有后续模块：

Director

Performance

Dialogue

Blocking

Camera

Continuity

Prompt Compiler

全部只能读取 Character Database。

禁止重新解析角色。

---

# Position

```
Script Parser

↓

Story Beat Engine

↓

Scene Breakdown

↓

Character Analysis Engine

↓

Director Engine
```

---

# Core Principle

一个角色。

必须同时拥有四种身份：

```
Narrative Identity

↓

Psychological Identity

↓

Physical Identity

↓

Performance Identity
```

缺少任何一种。

角色分析不完整。

---

# Character Database

每位角色建立唯一 Character ID。

```yaml
Character ID

Character Type

Priority

First Appearance

Last Appearance

Story Status
```

Character ID 全项目唯一。

不得重复。

---

# Character Type

自动分类：

```yaml
Protagonist

Deuteragonist

Antagonist

Supporting Character

Minor Character

Background Character

Voice Only

Off-screen Character
```

---

# Narrative Identity

建立角色在故事中的作用。

```yaml
Story Function

Narrative Goal

Story Arc

Conflict Type

Relationship Function

Character Growth
```

例如：

```
Protect Daughter

Hide Secret

Seek Revenge

Solve Case

Escape Reality
```

---

# Psychological Identity

建立人物心理模型。

```yaml
Core Desire

Core Fear

Belief

Weakness

Internal Conflict

External Conflict

Decision Pattern

Stress Response
```

这些数据。

后续 Dialogue Engine 和 Performance Engine 必须继承。

---

# Physical Identity

建立人物外部设定。

```yaml
Gender

Age

Nationality

Occupation

Height

Body Type

Skin Tone

Hair

Eyes

Face

Wardrobe

Accessories

Special Marks
```

整个项目保持一致。

---

# Performance Identity

建立演员层数据。

```yaml
Speaking Style

Voice Tone

Speech Rhythm

Walking Style

Standing Posture

Gesture Habit

Eye Contact Habit

Breathing Pattern

Facial Habit

Micro Expression Habit
```

例如：

```
说话前先停顿。

很少直视别人。

紧张时摸戒指。

生气时压低声音。

走路重心偏右。

```

这些不能靠 Prompt 临时生成。

必须永久记录。

---

# Relationship Map

建立角色关系网络。

```yaml
Character A

↓

Character B

Relationship

Trust Level

Conflict Level

History

Current Status
```

例如：

```
Father

↓

Daughter

Love

85

Conflict

20
```

随着剧情自动更新。

---

# Character Goal

建立三层目标。

```yaml
Long-term Goal

↓

Scene Goal

↓

Current Beat Goal
```

保证演员每一场戏都有明确行动目标。

---

# Character Emotion Model

建立完整情绪状态。

```yaml
Baseline Emotion

↓

Current Emotion

↓

Emotion Trigger

↓

Emotion Direction

↓

Expected Emotion
```

例如：

```
Calm

↓

Nervous

↓

Fear

↓

Anger

↓

Acceptance
```

---

# Character Arc

建立成长曲线。

```text
Beginning

↓

Challenge

↓

Failure

↓

Reflection

↓

Growth

↓

Transformation
```

后续所有表演必须遵循。

---

# Dialogue Identity

建立角色专属语言风格。

```yaml
Vocabulary

Sentence Length

Speaking Speed

Accent

Humor Style

Silence Habit

Favorite Expressions
```

禁止所有角色说话方式一致。

---

# Action Identity

建立动作习惯。

```yaml
Idle Pose

Default Walk

Default Run

Reaction Speed

Combat Style

Hand Preference

Movement Habit
```

例如：

```
左撇子。

坐下先扶椅背。

转身习惯向右。

```

---

# Character State Machine

建立永久角色状态。

```yaml
Current Location

Current Emotion

Current Action

Current Costume

Current Props

Current Health

Current Relationship

Current Objective
```

每个 Scene 自动更新。

---

# Character Package

最终输出：

```yaml
Character Profile

Narrative Identity

Psychological Identity

Physical Identity

Performance Identity

Relationship Map

Character Arc

Dialogue Identity

Action Identity

Current State
```

供：

Director Engine

Performance Engine

Dialogue Engine

Blocking Engine

统一读取。

---

# Validation Rules

检查：

✓ Character ID 是否唯一。

✓ Story Function 是否明确。

✓ 心理模型是否完整。

✓ 外观是否完整。

✓ 表演数据是否完整。

✓ Relationship 是否建立。

✓ Character Arc 是否存在。

✓ 当前状态是否初始化。

全部通过。

输出 Character Package。

---

# Lock Rules

以下数据默认锁定：

```yaml
Name

Age

Gender

Nationality

Appearance

Voice

Habit

Core Desire

Core Fear
```

剧情允许变化的数据：

```yaml
Emotion

Relationship

Goal

Health

Costume

Current State
```

任何 Engine 不得修改锁定字段。

---

# Final Principle

Character Analysis Engine 建立的不是人物设定。

而是一套可持续驱动导演、演员、摄影、对白与连续性系统的角色模型。

HDOS 后续所有镜头、所有表演、所有 Prompt，都必须基于 Character Database，而不是重新描述角色。

# End of File