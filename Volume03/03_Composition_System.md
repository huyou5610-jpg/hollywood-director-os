# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：03_Composition_System.md
# Priority：P3
# ============================================================

# Module

Composition System Engine

---

# Purpose

Composition System Engine（CSE）。

负责建立真人电影摄影中的构图语言（Composition Language）。

Hollywood Director OS 认为：

构图不是美术。

构图不是摄影技巧。

构图是：

**导演控制观众视线（Audience Attention）的核心工具。**

真正优秀的构图。

不是让画面漂亮。

而是让观众只能看导演希望他们看的地方。

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

Composition System

↓

Depth System

↓

Focus System

↓

Exposure System
```

---

# Core Principle

每一个构图必须回答：

```
观众第一眼看哪里？

↓

第二眼看哪里？

↓

第三眼发现什么？

↓

哪些信息应该隐藏？

↓

哪些信息应该强调？
```

如果不能控制观众视线。

构图失败。

---

# Composition Package

建立统一数据。

```yaml
Composition ID

Shot ID

Composition Type

Visual Priority

Eye Path

Balance Type

Negative Space

Narrative Purpose
```

---

# Composition Hierarchy

构图建立四层控制。

```text
Story

↓

Performance

↓

Composition

↓

Visual Decoration
```

画面永远服务故事。

---

# Composition Categories

统一分类。

```yaml
Centered

Rule of Thirds

Golden Ratio

Symmetrical

Asymmetrical

Diagonal

Triangular

Circular

Layered

Minimal

Dynamic
```

每个镜头。

只能拥有：

Primary Composition。

---

# Audience Eye Path

建立观众视线路径。

```text
Entry Point

↓

Primary Subject

↓

Secondary Subject

↓

Supporting Detail

↓

Exit Point
```

每个镜头。

必须建立完整路径。

---

# Subject Priority

统一主体等级。

```yaml
Primary Subject

Secondary Subject

Environment

Background Detail
```

任何镜头。

只能存在：

一个 Primary Subject。

---

# Balance Strategy

建立画面平衡。

```yaml
Perfect Balance

Emotional Balance

Intentional Imbalance

Visual Weight Shift
```

失衡。

必须具有导演意图。

---

# Negative Space

建立留白策略。

```yaml
None

Minimal

Controlled

Dominant
```

负空间用于：

```yaml
Loneliness

Isolation

Suspense

Power Difference

Psychological Pressure
```

---

# Frame Within Frame

允许：

画框中的画框。

例如：

```yaml
Door

Window

Mirror

Tunnel

Fence

Arch

Curtain
```

用于：

限制角色。

暗示命运。

强化观察感。

---

# Leading Lines

建立引导线。

```yaml
Road

Hallway

Rail

Wall

Light

Shadow

Architecture
```

所有引导线。

最终汇聚：

Primary Subject。

---

# Visual Weight

记录视觉重量。

```yaml
Character

Light

Color

Movement

Contrast

Depth
```

重量越高。

越容易吸引注意力。

---

# Layer Composition

建立空间层次。

```yaml
Foreground

Midground

Background
```

真人电影默认：

至少两层。

推荐三层。

---

# Headroom Rules

建立头部空间。

```yaml
Tight

Standard

Loose

Expressive
```

例如：

压迫：

Tight。

自由：

Loose。

---

# Look Room Rules

角色视线前方。

必须建立：

```yaml
Normal

Compressed

Extended
```

禁止：

角色看向画外。

却没有视觉空间。

---

# Walking Space

角色运动方向。

建立：

```yaml
Lead Space

Neutral

Restricted
```

动作戏。

必须预留：

运动空间。

---

# Symmetry Strategy

允许：

```yaml
Perfect Symmetry

Broken Symmetry

Near Symmetry
```

用于：

```yaml
Power

Religion

Order

Madness

Control
```

---

# Color Balance Hint

记录：

```yaml
Warm Area

Cold Area

Neutral Area

Contrast Area
```

供：

Color Engine。

统一调用。

---

# Composition Continuity

记录：

```yaml
Previous Frame

Current Frame

Next Frame
```

保持：

视觉连续。

禁止：

主体位置随机跳变。

---

# AI Composition Constraints

AI 视频增加：

```yaml
Stable Subject Position

Consistent Headroom

Consistent Eye Line

Consistent Layer

Stable Framing
```

降低：

AI 构图漂移。

---

# Composition Output

最终输出：

```yaml
Composition Profile

Eye Path

Subject Priority

Balance Strategy

Negative Space

Leading Lines

Layer Design

Frame Strategy

Continuity Profile
```

供：

Depth。

Focus。

Exposure。

统一读取。

---

# Validation Rules

检查：

✓ Eye Path 是否明确。

✓ Primary Subject 是否唯一。

✓ Negative Space 是否具有意义。

✓ Balance 是否符合剧情。

✓ Layer 是否完整。

✓ Leading Lines 是否有效。

✓ 构图是否突出表演。

✓ AI 是否可稳定保持构图。

任何失败。

禁止进入：

Depth System。

---

# Lock Rules

锁定：

```yaml
Composition Type

Eye Path

Primary Subject

Balance Strategy

Negative Space

Layer Design
```

允许：

后续模块补充：

```yaml
色彩

景深

曝光

镜头参数

后期裁切
```

禁止修改：

构图逻辑。

---

# Director Notes

自动生成：

```yaml
Attention Score

Composition Balance

Negative Space Analysis

Eye Path Quality

Performance Visibility

AI Composition Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

构图不是为了美。

构图是导演控制观众注意力的语言。

每一条线。

每一个留白。

每一个主体位置。

都必须回答同一个问题：

**观众现在应该看什么？**

如果构图不能精准引导观众视线。

那么无论画面多漂亮。

都不是合格的电影构图。

Composition System Engine 输出的是一套符合好莱坞真人电影工业标准、适配 AI 视频生成的构图系统，为后续景深、对焦、曝光和最终 Prompt Compiler 提供统一的视觉结构。

# End of File

# Next File

Volume03 / File：04_Depth_and_Layer.md