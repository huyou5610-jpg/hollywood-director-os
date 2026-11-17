# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume07
# Sound Engine
# File：02_Dialogue_System.md
# Priority：P7
# ============================================================

# Module

Dialogue System Engine

---

# Purpose

Dialogue System Engine（DSE）。

负责建立 Hollywood Director OS 的电影对白系统（Cinema Dialogue System）。

Hollywood Director OS 认为：

对白。

不是角色说的话。

而是：

**角色隐藏的话。**

真正优秀的电影对白。

观众听见的是语言。

理解的是人物。

感受到的是情绪。

Dialogue System 的职责。

就是建立：

**角色 → 情绪 → 信息 → 冲突 → 对白** 的完整电影对白体系。

---

# Position

```text
Sound Core

↓

Sound Theory

↓

Dialogue System

↓

Ambience Design

↓

Music Architecture

↓

Sound Emotion

↓

AI Sound Constraints

↓

Sound Validation
```

---

# Core Principle

每一句对白必须回答：

```text
为什么现在说？

↓

为什么必须由这个角色说？

↓

真正表达了什么？

↓

隐藏了什么？

↓

AI 是否能够稳定生成？
```

如果一句对白。

可以删除而剧情不变。

它应该被删除。

---

# Dialogue Philosophy

电影对白遵循：

```text
Story

↓

Character

↓

Emotion

↓

Conflict

↓

Dialogue

↓

Audience
```

对白。

永远服务人物。

---

# Dialogue Package

统一建立数据。

```yaml
Dialogue ID

Project ID

Sequence ID

Scene ID

Shot ID

Speaker

Listener

Narrative Purpose

Emotion Target

AI Constraint
```

---

# Dialogue Objectives

每一句对白至少承担一种职责。

```yaml
Advance Story

Reveal Character

Build Conflict

Deliver Information

Create Emotion

Increase Suspense

Foreshadow

Comic Relief

Relationship Development

Theme Expression
```

禁止：

无意义对白。

---

# Dialogue Hierarchy

建立统一控制层级。

```text
Story

↓

Narrative

↓

Character

↓

Emotion

↓

Conflict

↓

Dialogue
```

对白。

服从人物。

---

# Dialogue Categories

统一分类。

```yaml
Conversation

Conflict

Confession

Question

Explanation

Negotiation

Monologue

Voice Over

Inner Voice

Silence
```

统一管理。

---

# Dialogue Structure

统一句式结构。

```yaml
Setup

↓

Conflict

↓

Response

↓

Reaction

↓

Resolution
```

每段对白。

形成戏剧单元。

---

# Subtext System

对白必须包含潜台词。

统一分类。

```yaml
Truth Hidden

Emotion Hidden

Power Hidden

Fear Hidden

Love Hidden

Lie Hidden
```

观众。

理解真正含义。

---

# Information Density

统一信息密度。

```yaml
Low

Medium

High

Critical
```

避免：

信息堆积。

---

# Character Voice Identity

每个角色。

建立独立语言特征。

```yaml
Vocabulary

Sentence Length

Speaking Speed

Humor Style

Education Level

Accent

Silence Pattern
```

保证：

角色可识别。

---

# Dialogue Rhythm

同步：

```yaml
Performance

Editing

Music

Breathing

Silence
```

对白。

参与电影节奏。

---

# Interruptions

允许自然打断。

统一分类。

```yaml
Overlap

Cut Off

Pause

False Start

Self Correction
```

增强：

真实感。

---

# Silence Between Dialogue

对白之间。

统一沉默。

```yaml
Thinking

Embarrassment

Grief

Suspense

Reflection

Power Shift
```

沉默。

也是对白。

---

# Dialogue Perspective

统一对白视角。

```yaml
Objective

Subjective

Memory

Dream

Narration

Internal Monologue
```

保证：

叙事清晰。

---

# Dialogue Emotion Mapping

对白同步情绪。

```yaml
Love

Soft Pace

Fear

Broken Speech

Anger

Fast Rhythm

Grief

Long Pause

Hope

Warm Tone

Conflict

Sharp Delivery
```

对白。

表达情绪变化。

---

# Sound Integration

同步：

```yaml
Dialogue

Ambience

Music

Effects

Silence
```

避免：

对白被掩盖。

---

# AI Dialogue Constraints

针对 AI 视频。

建立：

```yaml
Stable Speaker Identity

Stable Lip Sync

Stable Speaking Pace

Stable Emotional Tone

Stable Dialogue Timing

Stable Character Voice
```

避免：

AI 角色口型、语气、身份漂移。

---

# Workflow

```text
Story

↓

Character

↓

Conflict

↓

Dialogue Writing

↓

Performance Planning

↓

Validation
```

对白。

来源于人物。

---

# Dialogue Output

统一输出。

```yaml
Dialogue Script

Subtext Layer

Emotion Layer

Timing

Speaker Identity

AI Constraint
```

供：

Ambience Design。

Music Architecture。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 是否推动剧情。

✓ 是否符合角色。

✓ 是否具有潜台词。

✓ 是否强化冲突。

✓ 是否保持节奏。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Ambience Design。

---

# Lock Rules

锁定：

```yaml
Dialogue Structure

Character Voice

Subtext

Emotion Mapping

Timing
```

允许：

后续模块补充：

```yaml
Ambient Mix

Music Layer

Performance Detail
```

禁止修改：

对白逻辑。

---

# Director Notes

自动生成。

```yaml
Dialogue Quality

Character Authenticity

Conflict Strength

Subtext Depth

Audience Engagement

AI Dialogue Stability
```

供导演、编剧、对白指导、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的对白。

不是角色说出了：

自己想什么。

而是：

观众听懂了。

角色没有说出口的东西。

Dialogue System Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway 等 AI 视频生成模型的电影对白系统，为 Ambience Design、Music Architecture、Sound Emotion、AI Sound Constraints 与 Prompt Compiler 提供统一、稳定、具有戏剧张力的对白架构。

