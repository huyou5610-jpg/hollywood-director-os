# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：02_Workflow.md
# Priority：P0
# ============================================================

# Module

Workflow

---

# Purpose

定义 Hollywood Director OS（HDOS）的唯一工作流程。

所有模块必须严格按照本流程执行。

禁止跳过流程。

禁止改变模块执行顺序。

禁止未完成上一阶段直接进入下一阶段。

系统始终遵循：

**先导演，后摄影；先设计，后编译。**

---

# HDOS Workflow

```
User Input
        │
        ▼
Script Engine
        │
        ▼
Director Engine
        │
        ▼
Performance Engine
        │
        ▼
Dialogue Engine
        │
        ▼
Blocking Engine
        │
        ▼
Camera Engine
        │
        ▼
Cinematography Engine
        │
        ▼
Lighting Engine
        │
        ▼
Action Engine
        │
        ▼
VFX Engine
        │
        ▼
Audio Engine
        │
        ▼
Continuity Engine
        │
        ▼
Prompt Compiler
        │
        ▼
Seedance Prompt
```

---

# Stage 01

Script Analysis

输入：

小说

剧本

对白

故事

创意

输出：

Story Package

包含：

Story

Character

Scene

Timeline

Conflict

Theme

Story Beat

---

# Stage 02

Director Planning

读取：

Story Package

建立：

Director Intent

Audience Emotion

Visual Style

Narrative Strategy

Rhythm

Pacing

输出：

Director Package

---

# Stage 03

Performance Planning

读取：

Director Package

建立：

Character Emotion

Performance Style

Body Language

Facial Expression

Eye Contact

Breathing

Pause

输出：

Performance Package

---

# Stage 04

Dialogue Planning

对白不是简单生成文字。

系统需要建立：

Dialogue Beat

Dialogue Emotion

Dialogue Pause

Dialogue Rhythm

Speech Speed

Stress

Voice Volume

Breathing Point

输出：

Dialogue Package

---

# Stage 05

Blocking Planning

建立：

Scene Layout

Actor Position

Movement Route

Screen Direction

Eye Line

Spatial Relation

Axis

Blocking Timeline

输出：

Blocking Package

---

# Stage 06

Camera Planning

摄影机根据导演意图工作。

建立：

Shot Size

Lens

Height

Distance

Movement

Motivation

Coverage

Transition

输出：

Camera Package

---

# Stage 07

Cinematography

建立：

Composition

Depth

Visual Hierarchy

Negative Space

Leading Line

Foreground

Background

Frame Balance

输出：

Cinematography Package

---

# Stage 08

Lighting Design

建立：

Lighting Source

Key Light

Fill Light

Back Light

Practical Light

Exposure

Contrast

Color Temperature

Mood

输出：

Lighting Package

---

# Stage 09

Action Design

如果镜头存在动作。

建立：

Action Beat

Action Rhythm

Action Physics

Recovery

Weight Shift

Interaction

输出：

Action Package

如果没有动作。

自动跳过。

---

# Stage 10

VFX Planning

判断：

是否需要：

Smoke

Fire

Rain

Snow

Fog

Explosion

Dust

Wind

Digital VFX

Practical FX

输出：

VFX Package

---

# Stage 11

Audio Planning

建立：

Dialogue Audio

Ambient

Footstep

Cloth

Weapon

Vehicle

Crowd

Weather

Silence

Music Suggestion

输出：

Audio Package

---

# Stage 12

Continuity Planning

系统读取上一镜状态。

建立：

Character Continuity

Camera Continuity

Emotion Continuity

Action Continuity

Dialogue Continuity

Lighting Continuity

Prop Continuity

Costume Continuity

Scene Continuity

输出：

Continuity Package

---

# Stage 13

Prompt Compilation

Prompt Compiler 统一读取：

Story Package

Director Package

Performance Package

Dialogue Package

Blocking Package

Camera Package

Cinematography Package

Lighting Package

Action Package

VFX Package

Audio Package

Continuity Package

编译：

Seedance Prompt

---

# Workflow Rules

## Rule 001

任何 Engine。

禁止直接读取剧本。

统一读取：

上一模块输出。

---

## Rule 002

所有模块。

必须输出结构化数据。

禁止输出自然语言 Prompt。

---

## Rule 003

所有模块。

允许增加细节。

禁止修改剧情。

---

## Rule 004

任何模块发现冲突。

停止编译。

返回：

Validation。

---

## Rule 005

Prompt Compiler。

永远最后执行。

---

# Data Flow

```
Input

↓

Parse

↓

Analyze

↓

Plan

↓

Design

↓

Validate

↓

Compile

↓

Optimize

↓

Output
```

禁止：

Input

↓

Prompt

---

# Validation Flow

每个阶段结束。

自动验证。

```
Structure Check

↓

Logic Check

↓

Continuity Check

↓

Director Check

↓

Visual Check

↓

Performance Check

↓

Prompt Check
```

全部通过。

进入下一阶段。

---

# Failure Strategy

任何模块失败。

系统不得继续。

返回上一阶段重新规划。

禁止生成存在逻辑错误的 Prompt。

---

# Final Workflow Principle

Hollywood Director OS 不以 Prompt 为中心。

而以电影导演工作流为中心。

Prompt 只是所有导演决策、演员表演、摄影设计、连续性规划和视觉语言统一后的最终编译结果。
