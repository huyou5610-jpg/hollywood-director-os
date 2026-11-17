# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：04_Seedance_Rules.md
# Priority：P0
# ============================================================

# Module

Seedance Native Generation Rules

---

# Purpose

本文件定义 Hollywood Director OS（HDOS）与 Seedance 2.0 的交互规则。

HDOS 不是为了生成"华丽 Prompt"。

而是为了生成：

**Seedance 最容易理解、最稳定、连续性最高、电影感最强的导演数据。**

因此。

所有 Engine。

最终必须遵循本规则。

---

# Core Principle

Seedance 接收的是：

Prompt。

实际上理解的是：

Scene。

Character。

Action。

Camera。

Environment。

Continuity。

因此。

HDOS 的目标不是增加描述。

而是降低模型理解成本。

---

# Rule 001

One Shot One Purpose

一个镜头。

只能表达一个主要信息。

禁止：

一个镜头同时完成：

介绍人物。

推动剧情。

展示动作。

表达情绪。

解释世界观。

---

# Rule 002

One Action One Beat

每个 Beat。

只允许一个主要动作。

例如：

正确：

角色停下。

↓

看向门口。

↓

门打开。

↓

角色后退。

错误：

角色奔跑。

转身。

开枪。

说话。

跳跃。

全部同时发生。

---

# Rule 003

One Camera Motivation

摄影机运动。

一次只有一个理由。

例如：

Follow

Reveal

Push Emotion

Observe

Track

禁止：

Push + Orbit + Crane 同时进行。

---

# Rule 004

Natural Performance

真人演员。

优先：

自然动作。

真实停顿。

真实呼吸。

真实重心。

禁止：

动漫式高速连续动作。

---

# Rule 005

Readable Prompt

Prompt 必须符合阅读逻辑。

按照：

Scene

↓

Character

↓

Action

↓

Performance

↓

Camera

↓

Lighting

↓

Environment

↓

Mood

↓

Continuity

输出。

禁止随机排列。

---

# Rule 006

Character First

Prompt 第一主体。

永远是角色。

不是镜头。

不是光影。

不是特效。

---

# Rule 007

Environment Stable

场景默认保持稳定。

禁止：

每镜重新描述世界。

Scene State 自动继承。

---

# Rule 008

State Driven

Prompt 不描述结果。

Prompt 描述状态。

例如：

不要写：

男主完成挥拳。

应该写：

男主右拳已完成约80%的挥击动作，身体重心压向左脚，惯性仍在继续。

---

# Rule 009

Performance Before Camera

任何镜头。

先确定演员。

再确定摄影机。

摄影机不能主导表演。

---

# Rule 010

Visual Simplicity

Prompt 应避免：

重复修饰词。

重复风格词。

重复电影名。

重复镜头词。

保持表达清晰。

---

# Rule 011

Implicit Continuity

默认继承：

上一镜：

人物。

服装。

站位。

情绪。

动作。

摄影机。

环境。

无需重复全部描述。

仅描述发生变化部分。

---

# Rule 012

No Prompt Decoration

禁止：

大量堆叠：

masterpiece

best quality

8k

ultra detailed

cinematic masterpiece

award winning

这些内容。

不能代替导演语言。

---

# Rule 013

Visual Priority

Prompt 必须明确：

Primary Subject

Secondary Subject

Background

确保模型知道：

第一眼看哪里。

---

# Rule 014

Real World Physics

真人剧默认遵循：

人体动力学。

重力。

惯性。

速度变化。

重量转移。

镜头运动规律。

除非：

剧本明确包含超自然设定。

---

# Rule 015

Editing Friendly

所有镜头。

必须考虑：

后期剪辑。

每个镜头必须拥有：

Start State

Middle Beat

End State

方便自然衔接。

---

# Prompt Assembly Order

Prompt Compiler 必须按照以下顺序组装：

```
Scene

↓

Character

↓

Current State

↓

Performance

↓

Action

↓

Camera

↓

Composition

↓

Lighting

↓

Environment

↓

Sound

↓

Continuity

↓

Director Style
```

禁止打乱顺序。

---

# HDOS Native Prompt Standard

Prompt 不使用关键词堆叠。

而采用导演描述。

例如：

```
Character:
A middle-aged detective stands beside the rain-soaked window, shoulders slightly tense, breathing controlled, eyes fixed on the approaching vehicle.

Performance:
He hesitates briefly before speaking, his voice calm but restrained, masking growing suspicion.

Camera:
A slow dolly-in from medium shot to medium close-up emphasizes the shift in emotional pressure without distracting movement.

Lighting:
Cold overcast daylight mixes with soft interior practical lighting, creating subtle contrast across his face.

Continuity:
Maintain the body orientation, eye line, and emotional state established in the previous shot.
```

---

# Validation Rules

Prompt Compiler 输出前必须检查：

✓ 是否只有一个主体。

✓ 是否符合导演意图。

✓ 是否符合人物状态。

✓ 是否符合场景状态。

✓ 是否符合连续性。

✓ 是否符合真人表演规律。

✓ 是否符合摄影语言。

✓ 是否符合电影语言。

✓ 是否符合 Seedance 可解析逻辑。

全部通过。

允许输出。

---

# Final Principle

HDOS 不追求最长 Prompt。

HDOS 追求：

**最少歧义。**

**最高可执行性。**

**最高镜头连续性。**

**最符合电影导演思维。**

最终让 Seedance 理解的是一场真实拍摄，而不是一段关键词集合。

# End of File