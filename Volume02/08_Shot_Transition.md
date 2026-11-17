# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：08_Shot_Transition.md
# Priority：P2
# ============================================================

# Module

Shot Transition Engine

---

# Purpose

Shot Transition Engine（STE）。

负责建立整个电影镜头之间的衔接语言（Shot Transition）。

Hollywood Director OS 认为：

Transition 不是一个剪辑动作。

而是：

**上一镜头如何结束。**

**下一镜头如何开始。**

**观众如何自然接受信息转换。**

真正优秀的转场。

观众几乎感觉不到。

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

Shot Transition

↓

Lighting

↓

Editing
```

---

# Core Principle

每一次转场必须回答：

```
为什么切？

↓

为什么现在切？

↓

为什么切到这里？

↓

观众是否已经获得当前镜头全部信息？

↓

下一镜是否拥有新的价值？
```

否则。

禁止 Cut。

---

# Transition Package

建立：

```yaml
Transition ID

Previous Shot

Current Shot

Transition Type

Narrative Purpose

Emotion Purpose
```

---

# Transition Hierarchy

建立四层转场。

```text
Shot Transition

↓

Segment Transition

↓

Scene Transition

↓

Sequence Transition
```

不同层级。

采用不同策略。

---

# Transition Types

统一分类。

```yaml
Hard Cut

Match Cut

Action Cut

Reaction Cut

Eyeline Cut

Insert Cut

Cutaway

L Cut

J Cut

Fade

Fade To Black

Fade To White

Dissolve

Whip Transition

Invisible Cut

Long Take

Smash Cut

Graphic Match

Sound Bridge

Visual Bridge
```

必须指定：

Primary Transition。

---

# Hard Cut

默认方式。

适用于：

```yaml
Dialogue

Action

Performance

Normal Narrative
```

不是：

所有地方都适合。

---

# Match Cut

保持视觉连续。

例如：

```yaml
Shape

Movement

Direction

Lighting

Composition
```

上一镜：

门打开。

下一镜：

另一扇门打开。

观众自然接受。

---

# Action Cut

动作完成一半切。

例如：

```
挥拳开始

↓

切另一机位

↓

拳头命中
```

动作连续。

观众不会察觉剪辑。

---

# Reaction Cut

Hollywood 默认最高优先级。

例如：

```
角色A说：

"他死了。"

↓

立即切：

角色B反应。
```

真正重要的是：

Reaction。

不是对白。

---

# Eyeline Cut

根据视线切换。

例如：

```
角色看向窗外

↓

窗外景象
```

建立：

视觉因果。

---

# Insert Cut

插入：

关键细节。

例如：

```yaml
枪

钥匙

戒指

手机

照片

血迹
```

必须推动剧情。

禁止：

装饰性 Insert。

---

# Cutaway

用于：

```yaml
环境

群众

天气

监控

动物

时钟
```

缓解节奏。

隐藏剪辑。

建立空间。

---

# L Cut

画面先切。

声音后切。

适用于：

情绪延续。

对白延续。

---

# J Cut

声音先进入。

画面后进入。

适用于：

场景转换。

制造期待。

---

# Invisible Cut

建立：

无感剪辑。

例如：

```yaml
Passing Object

Dark Frame

Camera Whip

Foreground Wipe
```

观众几乎无法察觉。

---

# Long Take

允许：

整个 Segment。

一个镜头。

必须满足：

```yaml
Performance Ready

Blocking Stable

Camera Stable

Story Continuous
```

不能为了炫技。

---

# Transition Motivation

每一次切换。

必须拥有：

```yaml
Information

Emotion

Performance

Rhythm

Perspective

Space
```

没有 Motivation。

禁止切换。

---

# Transition Timing

记录：

```yaml
Cut Point

Early Cut

Late Cut

Hold Duration

Transition Buffer
```

保证：

节奏自然。

---

# Audio Transition

建立：

声音衔接。

```yaml
Dialogue Bridge

Music Bridge

Ambience Bridge

FX Bridge

Silence Bridge
```

声音。

优先于画面。

---

# Visual Transition

建立：

视觉衔接。

```yaml
Direction Match

Lighting Match

Composition Match

Color Match

Motion Match
```

画面不能：

突然跳变。

---

# Emotion Transition

记录：

```yaml
Previous Emotion

↓

Transition

↓

Current Emotion
```

例如：

```
Hope

↓

Silence

↓

Despair
```

剪辑必须服务：

情绪。

---

# Transition Density

自动控制：

```yaml
Frequent

Balanced

Sparse
```

避免：

切换过多。

导致疲劳。

---

# Transition Output

最终输出：

```yaml
Transition Plan

Transition Type

Transition Motivation

Cut Timing

Audio Bridge

Visual Bridge

Emotion Bridge

Transition Density
```

供：

Editing Engine。

直接执行。

---

# Validation Rules

检查：

✓ Transition 是否具有动机。

✓ Cut Timing 是否合理。

✓ Emotion 是否连续。

✓ Audio 是否连续。

✓ Visual 是否连续。

✓ Information 是否完整。

✓ Rhythm 是否一致。

✓ Director Intent 是否保持。

任何失败。

禁止进入：

Lighting Engine。

---

# Lock Rules

锁定：

```yaml
Transition Type

Cut Timing

Transition Motivation

Emotion Bridge
```

允许：

Editing Engine。

补充：

```yaml
具体帧数

剪辑节奏

音频淡入淡出

颜色过渡
```

禁止修改：

导演转场逻辑。

---

# Director Notes

自动生成：

```yaml
Cut Risk

Reaction Opportunity

Match Cut Suggestion

L Cut Suggestion

J Cut Suggestion

Invisible Cut Opportunity
```

供导演确认。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的转场。

不是让观众注意到：

"这里剪了一刀。"

而是让观众自然进入下一段情绪。

Transition 的本质不是剪辑。

而是：

**信息传递。**

**情绪延续。**

**空间连接。**

**导演思维的连续表达。**

Shot Transition Engine 输出的是一套符合好莱坞真人电影工业标准的镜头衔接语言，为 Editing Engine 提供完整、可执行的导演转场方案。

# End of File

# Next File

Volume02 / File：09_Director_Validation.md
