# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume03
# Cinematography Engine
# File：07_Camera_Continuity.md
# Priority：P3
# ============================================================

# Module

Camera Continuity Engine

---

# Purpose

Camera Continuity Engine（CCE）。

负责建立整个真人电影摄影系统中的摄影连续性（Camera Continuity）。

Hollywood Director OS 认为：

摄影连续性。

不是镜头参数保持一致。

真正需要保持连续的是：

**观众的视觉认知。**

摄影连续性的职责：

保证整个 Scene、Sequence 乃至整部电影的摄影语言统一。

---

# Position

```text
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

↓

Camera Continuity

↓

Virtual Camera
```

---

# Core Principle

每一次镜头切换必须回答：

```text
观众是否仍然知道：

自己在哪里？

↓

正在看谁？

↓

摄影风格是否突然改变？

↓

镜头是否属于同一部电影？

↓

空间是否连续？
```

如果答案是否。

摄影连续性失败。

---

# Continuity Package

建立统一数据。

```yaml
Continuity ID

Scene ID

Sequence ID

Camera Style

Lens Continuity

Movement Continuity

Composition Continuity

Lighting Continuity

Narrative Continuity
```

---

# Continuity Hierarchy

建立四层连续性。

```text
Project

↓

Sequence

↓

Scene

↓

Shot
```

上层定义规则。

下层执行规则。

---

# Camera Style Lock

每部作品建立统一摄影风格。

```yaml
Classical

Naturalistic

Documentary

Epic

Minimal

Stylized

Handheld

Invisible Camera
```

整个项目。

不得频繁切换。

---

# Lens Continuity

记录：

```yaml
Previous Lens

Current Lens

Next Lens
```

检查：

```yaml
Perspective

Compression

Emotional Distance

Field of View
```

避免：

焦段语言混乱。

---

# Movement Continuity

记录：

```yaml
Movement Type

Movement Speed

Movement Energy

Movement Direction
```

保证：

摄影运动拥有统一逻辑。

---

# Composition Continuity

检查：

```yaml
Headroom

Lead Room

Subject Position

Frame Balance

Eye Line Position
```

避免：

人物位置随机变化。

---

# Focus Continuity

统一记录：

```yaml
Focus Distance

Focus Style

Rack Focus Pattern

Attention Priority
```

保证：

观众注意力连续。

---

# Exposure Continuity

检查：

```yaml
Brightness

Contrast

Shadow

Highlight

Dynamic Range
```

避免：

镜头忽明忽暗。

---

# Color Continuity

建立：

```yaml
White Balance

Temperature

Dominant Color

Contrast Palette

Color Mood
```

供：

Color Engine。

统一使用。

---

# Camera Height Continuity

记录：

```yaml
Eye Level

Low Angle

High Angle

Overhead

Ground Level
```

禁止：

镜头高度无原因变化。

---

# Camera Distance Continuity

统一管理：

```yaml
Extreme Wide

Wide

Medium

Medium Close

Close

Extreme Close
```

镜头距离变化。

必须符合：

情绪递进。

---

# Perspective Continuity

统一视角。

```yaml
Objective

Observer

Character POV

Restricted POV

Omniscient
```

不得：

突然切换。

除非：

导演刻意设计。

---

# Motion Direction

记录：

```yaml
Screen Left

Screen Right

Forward

Backward

Toward Camera

Away Camera
```

必须保持：

运动连续。

---

# Scene Boundary

允许：

Scene 重置摄影语言。

建立：

```yaml
Previous Style

↓

Transition

↓

New Style
```

每一次重置。

必须具有：

导演理由。

---

# Sequence Consistency

Sequence 内统一：

```yaml
Lens Family

Movement Style

Composition Logic

Exposure Style

Camera Energy
```

形成：

完整摄影语言。

---

# AI Continuity Constraints

针对 AI 视频。

增加：

```yaml
Stable Lens

Stable Camera Height

Stable Perspective

Stable Motion Curve

Stable Composition

Stable Exposure

Stable Color
```

减少：

AI 镜头漂移。

---

# Continuity Output

最终输出：

```yaml
Camera Style

Lens Continuity

Movement Continuity

Composition Continuity

Focus Continuity

Exposure Continuity

Color Continuity

AI Continuity Profile
```

供：

Virtual Camera。

Lighting。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ 摄影风格是否统一。

✓ Lens 是否连续。

✓ Movement 是否连续。

✓ Composition 是否稳定。

✓ Focus 是否一致。

✓ Exposure 是否一致。

✓ Color 是否一致。

✓ AI 是否能够稳定连续生成。

任何失败。

禁止进入：

Virtual Camera Engine。

---

# Lock Rules

锁定：

```yaml
Camera Style

Continuity Profile

Lens Family

Movement Style

Composition Logic
```

允许：

Virtual Camera。

补充：

```yaml
Camera Rig

Render Camera

AI Camera Token

Physical Camera Metadata
```

禁止修改：

摄影连续性。

---

# Director Notes

自动生成：

```yaml
Continuity Score

Lens Drift Warning

Movement Drift Warning

Exposure Drift Warning

Color Drift Warning

AI Stability Report
```

供摄影指导审核。

---

# Final Principle

Hollywood Director OS 中。

真正优秀的摄影。

不会让观众意识到：

镜头已经换了。

观众只会感觉：

故事一直在流动。

Camera Continuity Engine 的职责。

就是保证整个作品从第一镜到最后一镜。

始终拥有统一、稳定、可信的电影摄影语言。

它不仅服务真实电影拍摄。

更是 AI 连续视频生成稳定性的核心基础。

# End of File

# Next File

Volume03 / File：08_Virtual_Camera_for_AI.md
