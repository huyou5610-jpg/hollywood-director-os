# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：04_Depth_and_Layer.md
# Priority：P3
# ============================================================

# Module

Depth and Layer Engine

---

# Purpose

Depth and Layer Engine（DLE）。

负责建立真人电影摄影中的空间深度（Depth）与视觉层次（Layer）。

Hollywood Director OS 认为：

景深不是虚化背景。

层次不是把东西摆成前中后景。

真正的 Depth。

是：

**建立真实可信的三维空间。**

真正的 Layer。

是：

**控制观众在空间中的阅读顺序。**

优秀摄影。

首先让观众相信：

角色真的存在于那个世界。

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

Depth & Layer

↓

Focus System

↓

Exposure System
```

---

# Core Principle

每一个镜头必须回答：

```
空间有几层？

↓

人物位于哪一层？

↓

观众应该感受到多大的空间？

↓

背景应该参与叙事吗？

↓

景深是否服务故事？
```

如果空间没有层次。

画面就是平的。

---

# Depth Package

建立统一数据。

```yaml
Depth ID

Shot ID

Depth Strategy

Layer Count

Subject Layer

Background Layer

Narrative Purpose
```

---

# Depth Hierarchy

建立四层决策。

```text
Story

↓

Emotion

↓

Spatial Depth

↓

Lens & Aperture
```

禁止：

先决定虚化。

再决定故事。

---

# Layer Categories

统一层次定义。

```yaml
Foreground

Near Foreground

Midground

Background

Far Background
```

系统默认：

至少：

Foreground + Subject + Background。

---

# Depth Strategy

建立空间策略。

```yaml
Flat

Moderate

Deep

Compressed

Extreme Depth
```

不同类型：

对应不同戏剧效果。

---

# Narrative Purpose

景深必须服务一个目标。

```yaml
Character Isolation

Relationship

Reveal Environment

Guide Attention

Hide Information

Increase Scale

Psychological Distance
```

禁止：

为了电影感而虚化。

---

# Foreground Design

前景承担：

```yaml
Frame Subject

Create Depth

Occlusion

Reveal

Transition

Environmental Context
```

允许：

树枝。

门框。

玻璃。

人群。

栏杆。

增加真实空间。

---

# Midground Design

中景承担：

```yaml
Primary Performance

Dialogue

Action

Interaction
```

默认：

主角所在层。

---

# Background Design

背景承担：

```yaml
Environment

Story Context

Movement

Light Source

Secondary Narrative
```

背景不能：

毫无信息。

也不能：

抢戏。

---

# Layer Relationship

建立层级关系。

```yaml
Foreground Weight

Midground Weight

Background Weight
```

视觉重心。

始终位于：

Midground。

---

# Spatial Compression

统一记录。

```yaml
Expanded Space

Balanced Space

Compressed Space
```

由：

Lens Engine。

共同控制。

---

# Subject Separation

人物必须从背景分离。

方法包括：

```yaml
Depth

Light

Color

Contrast

Movement

Focus
```

禁止：

人物融入背景。

---

# Occlusion Strategy

允许：

遮挡设计。

例如：

```yaml
Door Frame

Window

People

Plants

Vehicle

Shadow
```

遮挡必须：

增强真实感。

不是遮住主体。

---

# Environmental Depth

建立环境深度。

```yaml
Atmospheric Perspective

Fog

Rain

Smoke

Dust

Light Beam
```

增加空间感。

同时服务叙事。

---

# Motion Layer

动态层次。

记录：

```yaml
Foreground Motion

Subject Motion

Background Motion
```

例如：

```
前景：

树叶摆动

↓

人物：

缓慢前进

↓

背景：

车辆经过
```

空间立即成立。

---

# Depth Progression

记录镜头中的深度变化。

例如：

```text
Deep

↓

Compressed

↓

Deep
```

用于：

心理变化。

剧情推进。

---

# AI Layer Constraints

针对 AI 视频。

增加限制。

```yaml
Stable Foreground

Stable Subject

Stable Background

No Layer Jump

Consistent Depth
```

避免：

背景闪烁。

人物穿模。

空间漂移。

---

# Depth Output

最终输出：

```yaml
Depth Strategy

Layer Design

Foreground Plan

Background Plan

Subject Separation

Spatial Compression

Environmental Depth

AI Layer Constraint
```

供：

Focus。

Exposure。

Lighting。

统一调用。

---

# Validation Rules

检查：

✓ 是否建立三维空间。

✓ Layer 是否完整。

✓ 主体是否清晰。

✓ 前景是否具有意义。

✓ 背景是否参与叙事。

✓ Depth 是否符合导演意图。

✓ AI 是否可稳定生成。

任何失败。

禁止进入：

Focus System。

---

# Lock Rules

锁定：

```yaml
Depth Strategy

Layer Design

Subject Layer

Foreground Plan

Background Plan
```

允许：

后续模块补充：

```yaml
景深参数

光圈

雾效

色彩层次

光照层次
```

禁止修改：

空间设计逻辑。

---

# Director Notes

自动生成：

```yaml
Depth Score

Layer Complexity

Foreground Quality

Background Quality

Spatial Realism

AI Stability
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正的电影空间。

不是靠广角创造。

而是靠层次创造。

观众看到的不只是一个人物。

而是一个真实存在、可以呼吸、可以进入的世界。

Depth and Layer Engine 输出的是一套符合好莱坞真人电影摄影标准、兼容 AI 视频生成的空间层次系统，为 Focus、Exposure、Lighting 与最终 Director Execution Sheet 提供稳定的三维视觉基础。

# End of File

# Next File

Volume03 / File：05_Focus_Control.md
