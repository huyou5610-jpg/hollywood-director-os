# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：01_Lens_System.md
# Priority：P3
# ============================================================

# Module

Lens System Engine

---

# Purpose

Lens System Engine（LSE）。

负责根据 Director Engine 与 Cinematography Core 的决策，为每一个镜头选择最合适的镜头语言（Lens Language）。

Hollywood Director OS 认为：

镜头（Lens）不是放大画面的工具。

而是：

**改变观众心理距离的工具。**

同一个演员。

不同焦段。

会产生完全不同的戏剧意义。

Lens System 的目标不是选择焦距。

而是建立：

**情绪距离（Emotional Distance）**。

---

# Position

```
Director Engine

↓

Cinematography Core

↓

Lens System

↓

Camera Movement

↓

Composition

↓

Depth

↓

Focus

↓

Exposure
```

---

# Core Principle

每一次镜头选择必须回答：

```
观众应该离角色多近？

↓

观众应该看到多少环境？

↓

空间应该真实还是压缩？

↓

情绪应该被放大还是克制？

↓

镜头是否符合导演意图？
```

---

# Lens Package

建立统一 Lens 数据。

```yaml
Lens ID

Shot ID

Lens Type

Focal Length

Perspective Type

Compression Level

Distortion Level

Narrative Purpose
```

---

# Lens Hierarchy

建立四层选择逻辑。

```text
Story

↓

Emotion

↓

Perspective

↓

Lens

```

禁止：

先决定焦段。

后决定故事。

---

# Lens Categories

统一镜头分类。

```yaml
Ultra Wide

Wide

Normal

Portrait

Telephoto

Super Telephoto

Macro
```

每个镜头。

必须拥有唯一 Primary Lens。

---

# Narrative Purpose

镜头必须服务一个目标。

```yaml
Reveal Space

Observe Character

Create Intimacy

Build Isolation

Increase Pressure

Hide Information

Observe Action

Enhance Scale

Compress Relationship
```

---

# Emotional Distance

建立观众距离。

```yaml
Detached

Observational

Personal

Intimate

Psychological
```

例如：

远景。

通常：

Detached。

特写。

通常：

Intimate。

---

# Perspective Mapping

不同镜头产生不同心理。

```yaml
Ultra Wide

↓

Environment First

Wide

↓

Relationship

Normal

↓

Natural Human Vision

Portrait

↓

Character Emotion

Telephoto

↓

Observation

Macro

↓

Detail
```

Lens 不只是画面大小。

而是叙事方式。

---

# Space Compression

建立空间关系。

```yaml
Expanded

Natural

Compressed
```

例如：

广角。

扩大空间。

长焦。

压缩空间。

空间变化必须具有戏剧目的。

---

# Distortion Strategy

允许：

```yaml
None

Minimal

Controlled

Expressive
```

默认：

真人剧禁止夸张畸变。

除非：

梦境。

心理幻觉。

极端情绪。

---

# Character Priority

建立人物拍摄策略。

```yaml
Environment First

Character Equal

Character Dominant

Emotion Dominant
```

例如：

爱情戏。

Emotion Dominant。

动作戏。

Character Equal。

---

# Multi Character Lens

多人场景建立：

```yaml
Single Focus

Dual Focus

Deep Composition

Layer Focus
```

镜头必须保证：

观众知道谁最重要。

---

# Lens Continuity

统一记录：

```yaml
Previous Lens

Current Lens

Next Lens

Transition Logic
```

禁止：

无意义焦段跳跃。

例如：

```
24mm

↓

200mm

↓

28mm
```

若无导演动机。

自动报警。

---

# Lens Progression

建立焦段推进。

例如：

```text
Wide

↓

Normal

↓

Portrait

↓

Close

```

用于：

情绪递进。

或：

```text
Close

↓

Normal

↓

Wide

```

用于：

情绪释放。

---

# AI Lens Constraints

针对 AI 视频。

增加约束。

```yaml
Lens Stable

Perspective Stable

Face Consistency

Environment Consistency

Depth Stable
```

避免：

AI 镜头漂移。

---

# Lens Recommendation Matrix

| Dramatic Purpose | Lens Strategy |
|------------------|---------------|
| 建立空间 | Wide |
| 建立人物关系 | Normal |
| 强调情绪 | Portrait |
| 制造压迫 | Telephoto |
| 展示细节 | Macro |
| 表现孤独 | Wide + Negative Space |
| 表现亲密 | Portrait Close |

---

# Lens Output

最终输出：

```yaml
Lens Profile

Perspective

Emotional Distance

Compression Strategy

Distortion Strategy

Character Priority

Lens Continuity

AI Lens Constraints
```

供：

Camera Movement。

Composition。

Depth。

统一调用。

---

# Validation Rules

检查：

✓ Lens 是否符合 Director Intent。

✓ Emotional Distance 是否正确。

✓ 空间压缩是否合理。

✓ Perspective 是否统一。

✓ 焦段变化是否连续。

✓ AI 是否能够稳定生成。

✓ 是否符合真人电影语言。

任何失败。

禁止进入：

Camera Movement。

---

# Lock Rules

锁定：

```yaml
Lens Type

Perspective

Emotional Distance

Compression Strategy

Lens Continuity
```

允许：

Camera Engine。

补充：

```yaml
真实焦距

光圈

滤镜

镜头品牌

呼吸补偿
```

禁止修改：

Lens Narrative Purpose。

---

# Director Notes

自动生成：

```yaml
Lens Consistency

Perspective Warning

Compression Suggestion

Emotion Distance Analysis

Lens Transition Risk

AI Stability Score
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

镜头不是光学器材。

镜头是一种叙事语言。

摄影指导选择的不是：

50mm。

85mm。

还是135mm。

真正选择的是：

**观众距离角色有多远。**

**观众是否能够进入角色内心。**

Lens System Engine 输出的是一套符合好莱坞真人电影摄影标准、适配 AI 视频生成的镜头语言系统，为后续 Camera Movement、Composition 与 Depth Engine 提供统一的视觉基础。

# End of File

# Next File

Volume03 / File：02_Camera_Movement.md
