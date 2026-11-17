# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume02
# Director Engine
# File：03_Camera_Language.md
# Priority：P2
# ============================================================

# Module

Camera Language Engine

---

# Purpose

Camera Language Engine（CLE）。

负责将 Shot Design Engine 输出的镜头目标，转换为真正具有电影语言的摄影方案。

Camera Language 不决定：

故事。

人物。

情绪。

它负责：

**如何让摄影机成为观众的眼睛。**

摄影机不是记录器。

摄影机本身就是叙事者。

---

# Position

```
Director Core

↓

Director Intent

↓

Shot Design

↓

Camera Language Engine

↓

Blocking

↓

Coverage

↓

Lighting

↓

Editing
```

---

# Core Principle

摄影机每一次存在。

必须回答：

```
为什么在这里？

↓

为什么现在移动？

↓

为什么现在停止？

↓

观众此刻应该看到什么？

↓

观众此刻不应该看到什么？
```

任何镜头。

不能回答。

立即删除。

---

# Camera Package

每一个 Shot 建立：

```yaml
Camera ID

Shot ID

Camera Role

Camera Motivation

Camera Position

Camera Height

Camera Distance

Camera Angle

Movement Type

Lens Strategy
```

---

# Camera Role

摄影机承担一种角色。

```yaml
Observer

Participant

Witness

Character POV

Hidden Observer

Narrator

Objective Camera

Subjective Camera
```

整个 Shot。

只能存在一个 Primary Role。

---

# Camera Motivation

摄影机只能因为以下原因移动。

```yaml
Reveal Information

Follow Character

Increase Emotion

Guide Attention

Create Suspense

Show Relationship

Build Scale

Hide Information
```

禁止：

为了炫技运镜。

---

# Camera Position

建立空间位置。

```yaml
Front

Rear

Left

Right

Diagonal

Overhead

Ground Level

Behind Object
```

所有位置。

必须服从：

Blocking。

---

# Camera Height

建立摄影高度。

```yaml
Eye Level

Low Angle

High Angle

Ground Level

Shoulder Level

Waist Level

Ceiling Level

Drone Level
```

高度改变。

必须具有戏剧意义。

---

# Camera Distance

摄影距离。

```yaml
Extreme Long

Long

Full

Medium

Close

Extreme Close
```

距离变化。

代表：

情绪变化。

信息变化。

关系变化。

---

# Camera Angle

摄影角度。

```yaml
Neutral

High

Low

Dutch

Top Down

Bottom Up

Profile

Three Quarter
```

禁止：

随机倾斜。

---

# Lens Strategy

摄影机读取：

Shot Design 的 Lens Hint。

建立：

```yaml
Wide Lens

Normal Lens

Portrait Lens

Telephoto

Macro
```

镜头选择。

服务：

导演表达。

而不是画面效果。

---

# Movement Language

统一运动语言。

```yaml
Static

Pan

Tilt

Dolly

Truck

Push In

Pull Out

Crane

Handheld

Steadicam

Gimbal

Orbit

Zoom

Whip Pan
```

每一种运动。

必须拥有：

Narrative Reason。

---

# Camera Speed

记录：

```yaml
Start Speed

Peak Speed

End Speed
```

禁止：

速度突变。

除非：

剧情需要。

---

# Camera Rhythm

建立摄影节奏。

```yaml
Still

↓

Slow

↓

Medium

↓

Fast

↓

Still
```

摄影节奏。

必须同步：

Scene Rhythm。

---

# Camera Focus

定义焦点变化。

```yaml
Primary Focus

Secondary Focus

Focus Shift

Rack Focus

Deep Focus

Selective Focus
```

观众注意力。

由 Focus 控制。

---

# Eye Path Design

建立观众视线路径。

```yaml
Entry Point

↓

Primary Subject

↓

Secondary Subject

↓

Exit Point
```

禁止：

画面没有视觉中心。

---

# Reveal Strategy

摄影机控制信息释放。

```yaml
Immediate Reveal

Delayed Reveal

Partial Reveal

Hidden Reveal

Progressive Reveal
```

例如：

凶手。

可以只露：

影子。

手。

鞋。

不露全脸。

---

# Camera Emotion

摄影机表达情绪。

```yaml
Distance

↓

Movement

↓

Composition

↓

Lens

↓

Lighting Support
```

例如：

孤独：

```
固定镜头

远景

负空间

慢节奏
```

压迫：

```
近景

推镜

长焦

低机位
```

---

# Camera Continuity

建立摄影连续性。

```yaml
Camera Side

Axis

Facing Direction

Movement Direction

Lens Continuity

Height Continuity
```

供：

180° Rule。

Continuity Engine。

共同使用。

---

# Camera Package Output

最终输出：

```yaml
Camera Role

Camera Position

Camera Height

Camera Angle

Movement Language

Lens Strategy

Focus Strategy

Reveal Strategy

Eye Path

Camera Continuity
```

供：

Blocking Engine。

Coverage Engine。

Lighting Engine。

统一调用。

---

# Validation Rules

检查：

✓ Camera Role 是否明确。

✓ Movement 是否具有动机。

✓ Focus 是否唯一。

✓ Eye Path 是否连续。

✓ Camera Continuity 是否完整。

✓ Axis 是否一致。

✓ Lens 是否符合 Intent。

✓ Camera 是否服务故事。

任何失败。

禁止进入：

Blocking Engine。

---

# Lock Rules

锁定：

```yaml
Camera Role

Movement Motivation

Reveal Strategy

Eye Path

Camera Continuity
```

允许：

后续模块补充：

```yaml
摄影参数

曝光

景深

防抖方式

设备类型
```

禁止修改：

摄影语言。

---

# Director Notes

自动生成：

```yaml
Primary Camera

Reaction Camera

Coverage Risk

Axis Warning

Focus Suggestion

Movement Suggestion
```

供导演审核。

---

# Final Principle

Hollywood Director OS 中。

摄影机不是记录现实。

摄影机负责控制观众如何理解现实。

Camera Language Engine 输出的不是摄影参数。

而是一套具有电影叙事能力的摄影语言系统。

摄影机必须始终服从：

故事。

角色。

情绪。

导演意图。

而不是画面本身。

# End of File

# Next File

Volume02 / File：04_Blocking_System.md
