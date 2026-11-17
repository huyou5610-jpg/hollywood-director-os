# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume01
# Script Engine
# File：00_Script_Parser.md
# Priority：P1
# ============================================================

# Module

Script Parser

---

# Purpose

Script Parser（SP）。

是整个 Hollywood Director OS 的第一个业务模块。

系统接收到任何用户输入后。

禁止直接生成分镜。

禁止直接生成 Prompt。

禁止直接进入 Director Engine。

必须先完成：

**剧本解析（Script Parsing）**。

Script Parser 的职责不是阅读文字。

而是理解电影。

最终输出：

统一、标准化、结构化的 Story Package。

供后续所有 Engine 调用。

---

# Position

```
User Input

↓

Script Parser

↓

Story Package

↓

Story Beat

↓

Director Engine
```

---

# Input Support

系统支持：

```
Feature Screenplay

TV Series Script

Short Drama Script

Novel

Light Novel

Web Novel

Comic Script

Story Outline

Treatment

Beat Sheet

Dialogue Only

Narration Only

Idea

Markdown

TXT

DOCX

PDF

JSON
```

系统自动识别输入类型。

用户无需指定格式。

---

# Parser Principles

## Principle 01

Story Before Language

Parser 不分析文字。

Parser 分析：

故事。

人物。

冲突。

情绪。

目标。

---

## Principle 02

Meaning Before Sentence

优先理解：

一句话表达什么。

而不是：

一句话写了什么。

---

## Principle 03

Film Thinking

所有解析。

最终都必须能够转换为：

Scene。

Shot。

Performance。

Camera。

而不是停留在文学表达。

---

# Parsing Pipeline

```
Input

↓

Format Detection

↓

Text Cleaning

↓

Structure Analysis

↓

Story Extraction

↓

Scene Detection

↓

Character Detection

↓

Dialogue Detection

↓

Action Detection

↓

Emotion Detection

↓

Timeline Detection

↓

Story Package
```

---

# Stage 01

Format Detection

自动识别：

```
Novel

↓

Screenplay

↓

Outline

↓

Dialogue

↓

Mixed Format
```

不同格式。

采用不同解析策略。

---

# Stage 02

Text Cleaning

自动删除：

```
重复空格

HTML 标签

Markdown 控制符

非法字符

重复标题

无效编号
```

保留：

原始语义。

---

# Stage 03

Structure Analysis

建立：

```
Project

Episode

Chapter

Sequence

Scene

Paragraph

Sentence
```

形成树状结构。

---

# Stage 04

Story Extraction

提取：

```
Genre

Theme

Tone

Conflict

Story Goal

Ending Direction

Narrative Style
```

---

# Stage 05

Scene Detection

自动寻找：

场景边界。

依据：

```
Location Change

Time Change

Character Entry

Character Exit

Major Event

Narrative Shift
```

自动建立：

Scene ID。

---

# Scene Rules

如果：

地点改变。

默认：

新 Scene。

如果：

时间跨度较大。

默认：

新 Scene。

如果：

人物全部更换。

重新评估是否拆分 Scene。

---

# Stage 06

Character Detection

自动识别：

```
Main Character

Supporting Character

Background Character

Off-screen Character
```

建立：

Character ID。

所有角色。

唯一编号。

---

# Character Initialization

首次出现时建立：

```yaml
Character ID

Name

Gender

Approximate Age

Occupation

Appearance

Current Goal

Relationship

Speaking Style

Initial Emotion

Initial Position
```

---

# Stage 07

Dialogue Detection

识别：

```
Dialogue

Inner Monologue

Voice Over

Narration

Phone Call

Radio

Off-screen Voice
```

对白自动绑定：

Character ID。

---

# Stage 08

Action Detection

识别：

```
Major Action

Minor Action

Physical Interaction

Object Interaction

Environmental Interaction
```

动作自动建立：

Action Beat。

---

# Stage 09

Emotion Detection

建立：

Emotion Timeline。

例如：

```
Neutral

↓

Curious

↓

Concerned

↓

Fear

↓

Determined
```

每位角色。

独立维护。

---

# Stage 10

Timeline Detection

建立：

故事时间轴。

包括：

```
Story Time

Scene Time

Flashback

Flashforward

Parallel Action

Real Time
```

---

# Story Package Output

最终输出：

```yaml
Project

Genre

Theme

Tone

Episodes

Characters

Locations

Timeline

Story Beats

Scenes

Dialogue

Actions

Emotions

Conflicts

Narrative Structure
```

---

# Parsing Rules

## Rule 001

禁止修改剧情。

---

## Rule 002

禁止补充剧情。

---

## Rule 003

禁止删除剧情。

---

## Rule 004

允许：

补充结构。

不允许：

补充故事。

---

## Rule 005

每一句对白。

必须绑定：

Character ID。

---

## Rule 006

每一个动作。

必须绑定：

Actor。

Target。

Scene。

---

## Rule 007

每一个 Scene。

必须拥有：

Scene Goal。

否则：

标记：

Need Analysis。

---

# Scene Goal Detection

系统自动判断：

当前 Scene 属于：

```
Character Introduction

Relationship Building

Conflict

Information Delivery

Suspense

Comedy

Action

Romance

Transition

Climax

Ending
```

至少拥有一个目标。

---

# Story Beat Detection

自动建立：

```
Opening

↓

Setup

↓

Inciting Incident

↓

Rising Action

↓

Midpoint

↓

Crisis

↓

Climax

↓

Resolution
```

后续 Director Engine。

直接读取。

---

# Output Validation

Parser 输出前。

检查：

✓ Scene 是否完整。

✓ Character 是否唯一。

✓ Timeline 是否连续。

✓ 对白是否绑定角色。

✓ 动作是否绑定人物。

✓ Scene 是否拥有目标。

✓ Story Beat 是否存在。

全部通过。

输出：

Story Package。

---

# Final Principle

Script Parser 是整个 Hollywood Director OS 的基础。

它不是文字解析器。

而是电影理解引擎。

所有后续导演决策、演员表演、摄影设计、连续性规划与 Prompt 编译，都必须建立在 Script Parser 输出的统一 Story Package 之上。

# End of File