# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：05_Output_Template.md
# Priority：P0
# ============================================================

# Module

Director Output Template

---

# Purpose

本文件定义 HDOS（Hollywood Director OS）唯一允许使用的导演输出模板。

所有 Engine。

最终必须输出统一的数据结构。

禁止：

不同模块使用不同格式。

禁止：

自由发挥输出顺序。

禁止：

Prompt 优先于导演数据。

系统始终遵循：

**Director Data First → Prompt Last**

---

# Output Philosophy

系统输出的不是 Prompt。

而是一份完整的导演执行方案（Director Package）。

Prompt。

只是最后一个字段。

---

# Output Hierarchy

```
Project

↓

Episode

↓

Sequence

↓

Scene

↓

Shot

↓

Director Package

↓

Seedance Prompt
```

---

# Project Output

```yaml
Project Name:

Genre:

Theme:

Tone:

Target Platform:

Target Duration:

Aspect Ratio:

Language:

Reference Style:

Seedance Version:
```

---

# Episode Output

```yaml
Episode ID:

Episode Title:

Episode Goal:

Story Progress:

Total Scenes:

Estimated Duration:
```

---

# Sequence Output

```yaml
Sequence ID:

Sequence Function:

Narrative Goal:

Beginning:

Development:

Climax:

Resolution:
```

---

# Scene Output

```yaml
Scene ID:

Scene Name:

Scene Goal:

Location:

Time:

Weather:

Lighting Condition:

Mood:

Characters:

Story Function:
```

---

# Shot Output

每一个镜头固定使用以下模板。

禁止修改字段顺序。

---

## Shot Header

```yaml
Shot ID:

Shot Number:

Shot Type:

Estimated Duration:

Story Beat:

Director Intent:
```

---

## Narrative

```yaml
Narrative Purpose:

Audience Emotion:

Information Revealed:

Conflict Level:
```

---

## Character

```yaml
Primary Character:

Secondary Character:

Current Emotion:

Current Action:

Current Position:

Eye Direction:

Body Orientation:

Costume State:

Prop State:
```

---

## Blocking

```yaml
Actor Position:

Movement Route:

Relationship Distance:

Screen Direction:

180° Axis:

Eye Contact:

Focus Order:
```

---

## Performance

```yaml
Performance Style:

Facial Expression:

Micro Expression:

Body Language:

Gesture:

Breathing:

Pause:

Performance Notes:
```

---

## Camera

```yaml
Shot Size:

Lens:

Camera Height:

Camera Distance:

Movement:

Movement Motivation:

Camera Speed:

Focus Target:
```

---

## Cinematography

```yaml
Composition:

Foreground:

Middle Ground:

Background:

Depth of Field:

Visual Hierarchy:

Negative Space:

Leading Lines:
```

---

## Lighting

```yaml
Lighting Style:

Key Light:

Fill Light:

Back Light:

Practical Light:

Exposure:

Contrast:

Color Temperature:

Shadow Direction:
```

---

## Environment

```yaml
Location State:

Weather State:

Wind:

Smoke:

Fog:

Rain:

Dust:

Interactive Objects:
```

---

## Action

```yaml
Action Beat:

Physics:

Weight Shift:

Momentum:

Recovery:

Interaction:
```

---

## Dialogue

```yaml
Speaker:

Dialogue:

Emotion:

Speech Speed:

Volume:

Stress:

Breathing Point:

Pause Timing:
```

---

## Audio

```yaml
Ambient:

Footsteps:

Cloth:

Environment:

Special Effects:

Music Suggestion:

Silence:
```

---

## Continuity

```yaml
Previous Shot ID:

Inherited Character State:

Inherited Scene State:

Inherited Camera State:

Inherited Emotion:

Inherited Action:

Inherited Lighting:

State Changes:

End State:
```

---

## Director Notes

```yaml
Visual Focus:

Editing Suggestion:

Transition:

Risk Check:

Director Notes:
```

---

## Seedance Prompt

最后统一生成：

```text
[Seedance Prompt]
```

禁止：

任何 Engine。

提前输出。

---

# Priority Order

所有字段。

按照以下优先级生成。

```
P0

Story

↓

Director Intent

↓

Continuity

↓

Character State

↓

Scene State

-------------------

P1

Blocking

↓

Performance

↓

Camera

↓

Dialogue

-------------------

P2

Lighting

↓

Composition

↓

Environment

↓

Action

↓

Audio

-------------------

P3

Prompt
```

低优先级。

不得影响高优先级。

---

# Shot State Rule

每一个镜头。

必须包含：

```yaml
Start State

↓

Action Beat

↓

Performance Change

↓

Camera Change

↓

Emotion Change

↓

End State
```

禁止：

镜头没有结束状态。

---

# Continuity Rule

每个镜头。

自动输出：

```yaml
Inherited From Previous Shot

Changed During Current Shot

Locked For Next Shot
```

例如：

```yaml
Inherited

Standing beside the doorway.

Looking at Character B.

Holding the pistol in the right hand.

Breathing remains steady.

Changed

Raises the pistol.

Steps forward 0.8 meters.

Voice becomes firmer.

Locked

Weapon remains raised.

Body turned 15° left.

Camera ends on medium close-up.

Emotional state: determined.
```

下一镜。

必须默认读取：

Locked State。

---

# Output Validation

输出前。

自动检查：

```
Story Complete

Character Complete

Scene Complete

Blocking Complete

Performance Complete

Camera Complete

Lighting Complete

Dialogue Complete

Continuity Complete

Prompt Complete
```

全部完成。

允许输出。

---

# Template Extension Rule

允许增加字段。

禁止删除：

P0。

禁止改变：

字段顺序。

保证所有 Engine 都能读取统一结构。

---

# Final Principle

Hollywood Director OS 的所有模块。

最终只允许输出这一套统一导演模板。

任何 Prompt。

都必须来源于该模板。

任何 Seedance 生成。

都必须能够追溯到：

Story → Director → Performance → Camera → Continuity → Prompt。

禁止直接从故事跳到 Prompt。

# End of File