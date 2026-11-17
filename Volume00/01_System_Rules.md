# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume00
# System Core
# File：01_System_Rules.md
# Priority：P0
# ============================================================

# Module

System Rules

---

# Purpose

本文件定义 Hollywood Director OS（HDOS）所有模块必须遵循的最高级系统规则。

所有 Engine。

所有 State Machine。

所有 Compiler。

所有 Prompt。

均不得违反本规则。

System Rules 优先级最高。

---

# Rule Hierarchy

P0（System Rules）

↓

P1（Engine Rules）

↓

P2（Module Rules）

↓

P3（Prompt Rules）

↓

P4（Output Style）

低优先级禁止覆盖高优先级。

---

# Rule 001

Story Integrity

任何情况下：

禁止修改故事主线。

禁止增加主剧情。

禁止删除关键剧情。

禁止改变人物命运。

系统职责：

影视化。

不是改编剧情。

---

# Rule 002

Character Integrity

角色设定永久锁定。

包括：

姓名

年龄

身份

职业

性格

说话方式

行为习惯

能力

外貌

服装

发型

肤色

口音

动作习惯

任何镜头禁止刷新角色。

---

# Rule 003

Scene Integrity

进入一个 Scene 后：

默认保持：

空间一致。

天气一致。

时间一致。

建筑一致。

家具一致。

环境一致。

直到：

Scene Transition。

---

# Rule 004

Performance Integrity

演员表演必须连续。

例如：

上一镜：

轻笑。

下一镜：

禁止突然愤怒。

除非：

剧情发生变化。

---

# Rule 005

Camera Integrity

摄影机连续。

默认：

继承上一镜：

位置。

高度。

焦段。

方向。

轴线。

运动状态。

禁止：

镜头突然跳跃。

---

# Rule 006

Lighting Integrity

光照默认连续。

包括：

太阳方向。

室内光源。

曝光。

色温。

阴影方向。

HDR。

除非：

剧情改变。

---

# Rule 007

Time Integrity

时间连续。

例如：

白天。

下一镜：

不能突然黑夜。

除非：

剧本说明。

---

# Rule 008

Costume Integrity

人物：

服装。

发型。

饰品。

污渍。

伤口。

汗水。

血迹。

全部连续。

---

# Rule 009

Prop Integrity

所有道具。

建立唯一状态。

例如：

杯子：

已打碎。

下一镜：

禁止恢复。

枪：

已经掉落。

下一镜：

禁止重新出现在手里。

---

# Rule 010

Emotion Integrity

情绪。

连续。

上一镜：

压抑。

下一镜：

必须经过：

释放。

爆发。

恢复。

禁止：

直接切换。

---

# Rule 011

Action Integrity

动作连续。

上一镜：

举枪。

下一镜：

保持举枪结束姿态。

禁止：

重新站立。

重新摆Pose。

重新开始动作。

---

# Rule 012

Dialogue Integrity

对白连续。

禁止：

一句对白。

拆断。

禁止：

语气重置。

禁止：

情绪重置。

---

# Rule 013

Eye Contact Integrity

上一镜：

看向角色A。

下一镜：

默认保持。

直到：

视线改变。

---

# Rule 014

Screen Direction

人物屏幕方向。

永久记录。

例如：

左→右。

下一镜：

继续。

禁止：

反向。

---

# Rule 015

180 Degree Rule

建立轴线后：

禁止跨轴。

如果必须跨轴。

必须：

执行：

Axis Transition。

重新建立轴线。

---

# Rule 016

Blocking Integrity

上一镜：

人物距离：

1.8m。

下一镜：

默认保持。

除非：

移动。

---

# Rule 017

Spatial Integrity

人物世界坐标。

永久保存。

下一镜。

继续读取。

禁止：

刷新站位。

---

# Rule 018

Camera Motivation

任何运镜。

必须拥有导演理由。

例如：

Reveal

Follow

Emotion

Pressure

Discovery

Transition

禁止：

随机运镜。

---

# Rule 019

Visual Priority

任何镜头。

只能拥有：

一个 Primary Subject。

允许：

两个 Secondary Subject。

禁止：

所有主体抢画面。

---

# Rule 020

Natural Performance

真人演员。

优先：

自然。

真实。

克制。

细节。

禁止：

动漫式夸张。

---

# Rule 021

Film Language

所有输出。

必须符合：

电影语言。

而不是：

Prompt关键词堆积。

---

# Rule 022

Cinematic Editing

系统在设计镜头时。

必须考虑：

后期剪辑。

任何镜头。

必须能够：

自然剪切。

自然衔接。

自然转场。

---

# Rule 023

Seedance Optimization

所有设计。

最终目的：

提高：

Seedance：

稳定性。

一致性。

连续性。

电影感。

---

# Rule 024

Prompt Compilation Only

任何 Engine。

禁止输出最终 Prompt。

所有 Engine。

输出：

结构化导演数据。

最终：

统一交给：

Prompt Compiler。

---

# Rule 025

No AI Style

最终输出。

禁止出现：

Prompt Engineering。

关键词堆叠。

AI描述语言。

所有内容。

统一采用：

导演语言。

摄影语言。

演员指导语言。

电影工业标准语言。

---

# Global Execution Order

System Core

↓

Script Engine

↓

Director Engine

↓

Performance Engine

↓

Dialogue Engine

↓

Blocking Engine

↓

Camera Engine

↓

Cinematography Engine

↓

Lighting Engine

↓

Action Engine

↓

VFX Engine

↓

Continuity Engine

↓

Prompt Compiler

任何模块。

禁止跳级。

禁止绕过。

禁止直接输出 Prompt。

---

# Validation

每个 Engine 输出后必须自动执行：

Story Validation

↓

Character Validation

↓

Scene Validation

↓

Continuity Validation

↓

Camera Validation

↓

Performance Validation

↓

Prompt Validation

全部通过。

系统才允许进入下一模块。

---

# Final Principle

Hollywood Director OS 的目标不是生成一句 Prompt。

而是模拟一套真实电影制作流程。

Prompt 只是电影工业流程的最终编译结果，而不是系统工作的起点。