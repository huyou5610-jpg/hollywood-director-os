# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：06_Quality_Standard.md
# Priority：P0
# ============================================================

# Module

Quality Standard

---

# Purpose

本文件定义 Hollywood Director OS（HDOS）唯一质量验收标准。

所有 Engine。

所有 Module。

所有 Output。

最终必须经过 Quality Standard 验证。

任何未达到标准的数据。

禁止进入 Prompt Compiler。

---

# Quality Philosophy

HDOS 的目标不是生成更多内容。

而是生成：

更准确。

更稳定。

更连续。

更符合电影工业流程。

因此：

质量优先于数量。

一致性优先于复杂度。

导演逻辑优先于 Prompt 长度。

---

# Quality Architecture

```
Story Quality

↓

Director Quality

↓

Performance Quality

↓

Blocking Quality

↓

Camera Quality

↓

Cinematography Quality

↓

Lighting Quality

↓

Dialogue Quality

↓

Continuity Quality

↓

Prompt Quality
```

全部通过。

系统允许输出。

---

# Quality Level

系统统一采用五级质量标准。

```
S+

Hollywood Studio Level

-------------------

S

Professional Film Level

-------------------

A

Commercial Level

-------------------

B

Usable Level

-------------------

C

Need Revision
```

最终目标：

默认达到：

S。

---

# Story Quality

检查：

Story Goal

Story Beat

Conflict

Character Motivation

Narrative Logic

Information Delivery

Scene Purpose

Validation：

✓ 每个 Scene 是否推动剧情。

✓ 每个 Shot 是否服务 Story Beat。

✓ 是否存在无意义镜头。

---

# Director Quality

检查：

Director Intent

Audience Emotion

Visual Strategy

Narrative Rhythm

Scene Design

Validation：

✓ 导演目标是否明确。

✓ 每个镜头是否存在导演意图。

✓ 是否能够仅通过画面表达故事。

---

# Performance Quality

检查：

Emotion

Facial Expression

Micro Expression

Body Language

Eye Contact

Breathing

Pause

Validation：

✓ 情绪是否真实。

✓ 表演是否自然。

✓ 是否存在情绪跳变。

✓ 是否符合人物设定。

---

# Blocking Quality

检查：

Actor Position

Movement

Eye Line

Distance

Focus

Axis

Validation：

✓ 是否符合空间关系。

✓ 是否符合人物关系。

✓ 是否保持视觉清晰。

✓ 是否符合180°规则。

---

# Camera Quality

检查：

Shot Size

Lens

Movement

Motivation

Composition

Coverage

Validation：

✓ 运镜是否拥有明确目的。

✓ 是否存在多余运镜。

✓ 是否符合电影摄影语言。

---

# Cinematography Quality

检查：

Composition

Visual Hierarchy

Negative Space

Leading Line

Depth

Frame Balance

Validation：

✓ 主体是否明确。

✓ 阅读顺序是否正确。

✓ 是否具备电影画面层次。

---

# Lighting Quality

检查：

Lighting Logic

Exposure

Contrast

Shadow

Color Temperature

Mood

Validation：

✓ 光源是否合理。

✓ 情绪是否由光影强化。

✓ 是否保持连续性。

---

# Dialogue Quality

检查：

Dialogue Beat

Pause

Stress

Breathing

Speech Speed

Emotion

Validation：

✓ 是否符合人物身份。

✓ 是否符合情绪。

✓ 是否具有自然停顿。

---

# Continuity Quality

检查：

Character

Camera

Action

Emotion

Dialogue

Lighting

Environment

Props

Validation：

✓ 是否继承上一镜状态。

✓ 是否存在穿帮。

✓ 是否存在动作断裂。

✓ 是否存在镜头跳轴。

---

# Prompt Quality

检查：

Director Intent

Readability

Structure

Execution

Continuity

Seedance Compatibility

Validation：

✓ 是否容易理解。

✓ 是否避免歧义。

✓ 是否符合 Seedance 解析逻辑。

✓ 是否保持电影语言。

---

# Automatic Quality Score

系统自动计算：

```yaml
Story Score:

Director Score:

Performance Score:

Blocking Score:

Camera Score:

Lighting Score:

Dialogue Score:

Continuity Score:

Prompt Score:
```

最终生成：

```yaml
Overall Quality Score
```

---

# Quality Threshold

```
95~100

S+

----------------

90~94

S

----------------

80~89

A

----------------

70~79

B

----------------

<70

Reject
```

低于：

80。

禁止输出。

---

# Auto Repair Strategy

若任一模块低于标准。

系统自动进入：

```
Detect

↓

Locate

↓

Repair

↓

Validate

↓

Recalculate

↓

Continue
```

禁止：

带错误进入下一模块。

---

# Global Validation Checklist

输出前必须确认：

✓ 剧情完整。

✓ 导演意图明确。

✓ 演员表演自然。

✓ Blocking 合理。

✓ 摄影语言成立。

✓ 构图清晰。

✓ 光影统一。

✓ 对白自然。

✓ 连续性完整。

✓ Prompt 可执行。

全部通过。

允许输出。

---

# Final Principle

HDOS 不以 Prompt 长短作为质量标准。

唯一标准是：

**是否达到真实电影导演、摄影指导、演员导演和场记团队共同完成的工业化制作质量。**

质量评分贯穿整个系统。

任何模块不得绕过 Quality Standard。

# End of File