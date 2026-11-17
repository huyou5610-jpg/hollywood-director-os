# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：03_Input_Output.md
# Priority：P0
# ============================================================

# Module

Input & Output Specification

---

# Purpose

本文件定义 HDOS（Hollywood Director OS）的标准输入、内部数据格式及最终输出规范。

任何 Engine。

不得直接处理用户原始文本。

所有用户输入。

必须先标准化（Normalize）。

所有模块。

统一读取标准化数据。

---

# HDOS Processing Pipeline

```
User Input

↓

Normalize

↓

Structured Data

↓

Engine Processing

↓

Director Data

↓

Prompt Compilation

↓

Final Output
```

---

# Supported Input Types

系统支持以下输入：

### Type 01

Novel

小说。

长篇小说。

短篇小说。

网络小说。

轻小说。

---

### Type 02

Screenplay

电影剧本。

电视剧剧本。

短剧剧本。

广告脚本。

MV脚本。

---

### Type 03

Outline

故事大纲。

章节简介。

剧情简介。

人物设定。

---

### Type 04

Dialogue

对白。

独白。

采访。

聊天记录。

旁白。

---

### Type 05

Existing Storyboard

已有分镜。

导演脚本。

拍摄脚本。

镜头表。

---

### Type 06

Idea

一句创意。

一句描述。

一句故事。

关键词。

系统负责扩展为完整影视方案。

---

# Normalize Stage

所有输入。

统一转换为：

Story Package。

---

# Story Package Structure

```yaml
Project

Genre

Theme

Tone

Language

Target Duration

Episode Count

Story

Characters

Locations

Timeline

Conflict

Ending

Reference Style
```

---

# Character Package

每位角色建立唯一数据。

```yaml
Character ID

Name

Age

Gender

Nationality

Occupation

Appearance

Wardrobe

Hair

Face

Voice

Accent

Personality

Relationship

Goal

Fear

Habit

Body Language

Speaking Style

Current Emotion

Current Action

Current Position
```

整个项目期间。

Character ID 永不改变。

---

# Scene Package

每一个 Scene。

建立唯一 Scene ID。

```yaml
Scene ID

Scene Name

Location

Interior / Exterior

Time

Weather

Season

Mood

Lighting

Props

Environment

Scene Goal

Characters

Start State

End State
```

---

# Shot Package

每一个镜头。

建立唯一 Shot ID。

```yaml
Shot ID

Scene ID

Shot Order

Story Beat

Director Intent

Duration

Start State

End State
```

Shot ID 永久唯一。

禁止重复。

---

# Director Package

导演层数据。

```yaml
Director Goal

Audience Emotion

Narrative Function

Visual Strategy

Performance Strategy

Camera Strategy

Lighting Strategy

Rhythm Strategy

Transition Strategy
```

所有 Engine。

统一读取。

---

# Performance Package

演员数据。

```yaml
Emotion

Eye Contact

Facial Expression

Micro Expression

Breathing

Body Language

Gesture

Movement

Dialogue Emotion

Performance Notes
```

---

# Camera Package

摄影数据。

```yaml
Shot Size

Lens

Camera Height

Camera Distance

Movement

Movement Motivation

Camera Speed

Focus

DOF

Composition

Transition
```

---

# Lighting Package

灯光数据。

```yaml
Key Light

Fill Light

Back Light

Practical Light

Contrast

Exposure

Color Temperature

Lighting Motivation

Shadow Direction
```

---

# Action Package

动作数据。

```yaml
Action Beat

Action Type

Action Rhythm

Physics

Interaction

Weight Shift

Recovery

Impact
```

---

# Audio Package

声音数据。

```yaml
Dialogue

Ambient

Footstep

Cloth

Environment

Music

Silence

SFX

Dynamic Range
```

---

# Continuity Package

系统自动维护。

```yaml
Previous Shot

Current Shot

Character State

Camera State

Scene State

Prop State

Emotion State

Dialogue State

Lighting State

Axis State

Screen Direction

Movement Continuity
```

---

# Prompt Package

Prompt Compiler 唯一输入。

```yaml
Story

Director

Performance

Dialogue

Blocking

Camera

Lighting

Action

VFX

Audio

Continuity
```

禁止任何 Engine。

直接输出 Prompt。

---

# Final Output Structure

系统最终统一输出：

```text
Project

↓

Episode

↓

Scene

↓

Scene Goal

↓

Director Intent

↓

Story Beat

↓

Blocking

↓

Performance

↓

Camera

↓

Lighting

↓

Action

↓

Dialogue

↓

Audio

↓

Continuity Notes

↓

Seedance Prompt
```

---

# Output Rules

## Rule 001

输出顺序固定。

禁止改变。

---

## Rule 002

所有镜头。

必须包含：

Director Intent。

---

## Rule 003

所有镜头。

必须包含：

Continuity Notes。

说明：

当前镜头如何承接上一镜。

---

## Rule 004

所有 Prompt。

必须来源于结构化数据。

禁止直接拼接关键词。

---

## Rule 005

每个镜头输出两层内容：

### Layer 1

导演数据（Director Data）

用于检查。

编辑。

修改。

---

### Layer 2

Seedance Prompt

用于最终生成。

---

# Prompt Generation Principle

HDOS 永远不会从用户输入直接生成 Prompt。

而是：

```
Story

↓

Director Decision

↓

Performance Design

↓

Visual Design

↓

Continuity Verification

↓

Prompt Compilation

↓

Seedance Prompt
```

---

# Validation Before Output

任何输出前。

必须通过：

```
Story Validation

↓

Character Validation

↓

Scene Validation

↓

Performance Validation

↓

Camera Validation

↓

Lighting Validation

↓

Continuity Validation

↓

Prompt Validation
```

任何一项失败。

禁止输出最终 Prompt。

---

# Final Principle

用户输入的是故事。

HDOS 输出的是一套完整的电影导演方案。

Seedance Prompt 只是导演方案经过统一编译后的最终交付文件，而不是系统工作的核心目标。
