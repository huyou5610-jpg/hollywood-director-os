# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume12
# Audio Engine
# File：02_Dialogue_System.md
# Priority：P12
# ============================================================

# Module

Dialogue System Engine

---

# Purpose

Dialogue System Engine（DSE）。

负责建立 Hollywood Director OS 的电影对白系统（Cinema Dialogue System）。

Hollywood Director OS 认为：

真正优秀的对白。

不是：

角色说了很多。

而是：

**角色只说必须说的话。**

电影对白。

不是解释故事。

而是：

揭示人物。

推动剧情。

表达冲突。

制造潜台词。

建立情感。

Dialogue System 的职责。

就是建立：

**人物 → 冲突 → 潜台词 → 节奏 → 情绪 → 电影对白**

的完整电影对白体系。

---

# Position

```text
Audio Theory

↓

Dialogue System

↓

Music System

↓

Sound Design

↓

Audio Validation
```

---

# Core Principle

每一句对白必须回答：

```text
为什么必须说？

↓

是谁在说？

↓

真正想表达什么？

↓

观众能够理解潜台词吗？

↓

AI 是否能够稳定生成？
```

对白。

必须服务人物。

---

# Dialogue Philosophy

电影对白遵循：

```text
Character

↓

Conflict

↓

Subtext

↓

Dialogue

↓

Audience
```

对白。

塑造人物。

---

# Dialogue Package

统一建立对白数据。

```yaml
Dialogue ID

Project ID

Sequence ID

Scene ID

Character ID

Dialogue Type

Narrative Purpose

Emotion

Validation Status
```

---

# Dialogue Objectives

每一句对白至少承担一种职责。

```yaml
Advance Story

Reveal Character

Create Conflict

Express Emotion

Deliver Information

Build Relationship

Increase Suspense

Foreshadow

Theme Expression

Audience Immersion
```

禁止：

没有叙事价值的对白。

---

# Dialogue Hierarchy

统一控制层级。

```text
Story

↓

Character

↓

Conflict

↓

Dialogue

↓

Audience
```

对白。

服从人物。

---

# Dialogue Types

统一对白类型。

```yaml
Conversation

Conflict

Confession

Interrogation

Negotiation

Argument

Monologue

Voice Over

Narration

Inner Voice
```

采用：

电影工业标准分类。

---

# Character Voice

统一角色语言风格。

```yaml
Vocabulary

Sentence Length

Speaking Speed

Tone

Education Level

Cultural Background
```

每位角色。

拥有独立语言特征。

---

# Subtext System

统一潜台词设计。

```yaml
Truth

Hidden Intention

Emotion

Irony

Conflict

Unspoken Desire
```

真正的对白。

隐藏真实含义。

---

# Conflict Dialogue

对白冲突。

```yaml
Direct Conflict

Emotional Conflict

Ideological Conflict

Power Conflict

Relationship Conflict

Internal Conflict
```

冲突。

推动剧情。

---

# Emotional Dialogue

对白情绪。

```yaml
Love

Fear

Anger

Hope

Sadness

Joy

Anxiety

Determination
```

语言。

传递情绪。

---

# Information Delivery

信息表达。

```yaml
Exposition

Hint

Reveal

Secret

Foreshadow

Resolution
```

避免：

信息堆砌。

---

# Dialogue Rhythm

对白节奏。

```yaml
Pause

Overlap

Interrupt

Silence

Fast Exchange

Long Speech
```

对白。

参与电影节奏。

---

# Silence Between Dialogue

对白间静默。

```yaml
Thinking

Emotion

Pressure

Suspense

Reflection

Relationship
```

沉默。

也是对白。

---

# AI Dialogue Constraints

针对 AI 视频。

建立：

```yaml
Stable Character Voice

Stable Emotion

Stable Speaking Style

Stable Timing

Stable Identity

Stable Prompt Mapping
```

避免：

AI 人物说话风格漂移。

---

# Workflow

```text
Story

↓

Character

↓

Dialogue Writing

↓

Subtext Design

↓

Validation
```

对白。

来源于人物。

---

# Dialogue Output

统一输出。

```yaml
Dialogue Blueprint

Character Voice Profile

Subtext Report

Emotion Curve

Narrative Function

AI Constraint
```

供：

Music System。

Sound Design。

Audio Validation。

统一调用。

---

# Validation Rules

检查：

✓ 是否符合人物设定。

✓ 是否推动剧情。

✓ 是否具有潜台词。

✓ 是否表达真实情绪。

✓ 是否符合电影工业标准。

✓ 是否支持 AI 稳定生成。

任何失败。

禁止进入：

Music System。

---

# Lock Rules

锁定：

```yaml
Character Voice

Dialogue Logic

Subtext Structure

Narrative Function

Conflict Design
```

允许：

后续模块补充：

```yaml
Music

Sound Design

Validation
```

禁止修改：

对白逻辑。

---

# Director Notes

自动生成。

```yaml
Dialogue Quality

Character Authenticity

Subtext Depth

Narrative Strength

Industrial Readiness

AI Stability
```

供导演、编剧（Writer）、对白指导（Dialogue Coach）、声音指导（Supervising Sound Editor）、AI Supervisor 联合审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的电影对白。

不是：

角色说了很多。

而是：

观众听见一句话。

却理解了：

十句话。

因为：

电影真正打动人的。

不是对白本身。

而是：

**没有说出口的话。**

Dialogue System Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo、Runway、Luma、Pika、Hailuo 等 AI 视频生成模型的电影对白系统，为 Music System、Sound Design、Audio Validation 与 Prompt Compiler 提供统一、稳定、具有电影工业标准的对白设计框架。

