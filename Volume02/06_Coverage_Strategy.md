# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：06_Coverage_Strategy.md
# Priority：P2
# ============================================================

# Module

Coverage Strategy Engine

---

# Purpose

Coverage Strategy Engine（CSE）。

负责设计整个 Scene 的镜头覆盖方案（Coverage）。

Hollywood Director OS 认为：

Coverage 不是：

"多拍几个镜头。"

而是：

**保证导演拥有足够的信息、情绪、空间和剪辑选择权。**

Coverage 是导演给后期剪辑准备的素材策略。

而不是摄影清单。

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

Lighting

↓

Editing
```

---

# Core Principle

每一个 Coverage 必须回答：

```
为什么拍？

↓

给后期提供什么？

↓

如果删掉它，故事还能成立吗？

↓

它补充了什么信息？

↓

它是否拥有唯一价值？
```

如果不能回答。

该 Coverage 删除。

---

# Coverage Package

建立：

```yaml
Coverage ID

Scene ID

Segment ID

Coverage Type

Coverage Priority

Narrative Purpose
```

---

# Coverage Hierarchy

Coverage 分四级。

```
Master Coverage

↓

Primary Coverage

↓

Support Coverage

↓

Optional Coverage
```

其中：

Master。

必须存在。

---

# Coverage Types

系统统一分类。

```yaml
Master Shot

Wide Shot

Two Shot

Single

OTS

Insert

Reaction

Cutaway

POV

Tracking

Environmental

Transition
```

每一个 Coverage。

只能承担一种主要职责。

---

# Master Coverage

Master Shot 永远负责：

```yaml
Scene Geography

Character Position

Blocking

Movement

Scene Continuity
```

任何 Scene。

默认生成。

至少：

一个 Master。

---

# Primary Coverage

Primary Shot。

负责：

```yaml
Performance

Dialogue

Conflict

Emotion

Story Information
```

真人剧。

默认：

Primary Coverage。

数量最多。

---

# Support Coverage

用于补充：

```yaml
Reaction

Insert

Environment

Relationship

Details
```

不是：

主镜头。

而是：

增强叙事。

---

# Optional Coverage

可选镜头。

例如：

```yaml
Atmosphere

Symbolism

Visual Metaphor

Texture

Slow Motion
```

如果时间不足。

优先删除。

---

# Coverage Priority

系统自动排序。

```yaml
★★★★★

Story

★★★★★

Performance

★★★★★

Reaction

★★★★☆

Space

★★★★☆

Insert

★★★☆☆

Environment

★★☆☆☆

Style
```

风格。

永远最后。

---

# Coverage Logic

Coverage 必须遵守：

```
空间

↓

人物

↓

表演

↓

情绪

↓

细节

```

禁止：

一开始全部特写。

---

# Performance Coverage

演员优先。

建立：

```yaml
Dialogue Coverage

Reaction Coverage

Silence Coverage

Micro Expression Coverage

Body Language Coverage
```

Hollywood 默认：

Reaction > Dialogue。

---

# Reaction Coverage

系统自动判断：

何时必须拍 Reaction。

例如：

```yaml
Truth Reveal

Death

Proposal

Betrayal

Gunshot

Silence

Unexpected News
```

Reaction。

优先级：

最高。

---

# Insert Strategy

Insert。

必须具有：

叙事作用。

例如：

```yaml
Gun

Ring

Letter

Phone

Blood

Photo

Key

Door Handle
```

禁止：

无意义插入。

---

# Environmental Coverage

建立：

环境镜头。

用于：

```yaml
Location

Weather

Time

Crowd

Atmosphere

Transition
```

不能：

抢主戏。

---

# Coverage Density

建立覆盖密度。

```yaml
Sparse

Normal

Dense

Extensive
```

例如：

对白戏：

Normal。

动作戏：

Dense。

---

# Coverage Redundancy

自动检查：

是否重复。

例如：

三个：

一样的：

中景。

系统：

建议删除。

---

# Coverage Economy

导演必须考虑：

```yaml
Narrative Value

Editing Value

Performance Value

Production Cost
```

优先：

价值最高。

成本最低。

---

# Editing Support

每个 Coverage。

自动标记：

```yaml
Cut In

Cut Out

Reaction Match

L Cut

J Cut

Bridge
```

方便：

剪辑系统。

---

# Coverage Matrix

系统自动建立：

| 内容 | 是否覆盖 |
|------|----------|
| 空间 | ✓ |
| 主角 | ✓ |
| 配角 | ✓ |
| 动作 | ✓ |
| 情绪 | ✓ |
| Reaction | ✓ |
| 道具 | ✓ |
| 环境 | ✓ |
| 转场 | ✓ |

任何缺失。

自动报警。

---

# Coverage Output

最终输出：

```yaml
Coverage Plan

Coverage Priority

Coverage Density

Reaction Plan

Insert Plan

Environment Plan

Editing Support

Coverage Matrix
```

供：

Lighting。

Editing。

Prompt Compiler。

统一读取。

---

# Validation Rules

检查：

✓ Master 是否存在。

✓ Performance 是否覆盖。

✓ Reaction 是否完整。

✓ Insert 是否合理。

✓ Environment 是否建立。

✓ Coverage 是否重复。

✓ Coverage 是否符合 Director Intent。

✓ Coverage 是否满足剪辑需求。

任何失败。

禁止进入：

Lighting Engine。

---

# Lock Rules

锁定：

```yaml
Coverage Plan

Coverage Priority

Coverage Matrix

Reaction Plan
```

允许：

Lighting。

FX。

Prompt Compiler。

增加执行细节。

禁止修改：

Coverage 逻辑。

---

# Director Notes

自动生成：

```yaml
Coverage Missing

Reaction Missing

Insert Suggestion

Editing Flexibility

Production Efficiency

Coverage Risk
```

供导演确认。

---

# Final Principle

Hollywood Director OS 中。

Coverage 的目标不是：

拍得更多。

而是：

**拍得刚好。**

每一个镜头都必须拥有存在价值。

每一种 Coverage 都必须提高故事表达、演员表演或后期剪辑的质量。

真正优秀的导演，不会依赖更多镜头，而会依赖更精准的 Coverage。

Coverage Strategy Engine 输出的是一套符合好莱坞真人剧工业流程、可直接进入拍摄与剪辑阶段的镜头覆盖方案。

# End of File

# Next File

Volume02 / File：07_Shot_Rhythm.md
