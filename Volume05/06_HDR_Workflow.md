# ============================================================
# Hollywood Director OS for Seedance 2.0
# Version 2.0
# Volume05
# Color Pipeline Engine
# File：06_HDR_Workflow.md
# Priority：P5
# ============================================================

# Module

HDR Workflow Engine

---

# Purpose

HDR Workflow Engine（HWE）。

负责建立 Hollywood Director OS 的电影 HDR（High Dynamic Range）工作流系统。

Hollywood Director OS 认为：

HDR 不是让画面更亮。

不是让颜色更鲜艳。

真正优秀的 HDR。

是：

**让光拥有真实的能量。**

HDR 的职责不是制造视觉刺激。

而是：

**完整保留导演、摄影、灯光、色彩设计所创造的光影层次。**

---

# Position

```text
Color Pipeline Core

↓

Color Science

↓

Color Palette

↓

Color Script

↓

Color Emotion

↓

LUT System

↓

HDR Workflow

↓

ACES Pipeline

↓

AI Color Constraints

↓

Color Validation
```

---

# Core Principle

每一个 HDR 流程必须回答：

```text
为什么需要 HDR？

↓

HDR 强化了哪些光影关系？

↓

是否保护导演意图？

↓

是否兼容 SDR？

↓

AI 是否能够稳定输出？
```

如果 HDR 只是更亮。

Workflow 失败。

---

# HDR Package

统一建立数据。

```yaml
HDR ID

Project ID

Scene ID

Shot ID

HDR Profile

Peak Brightness

Shadow Floor

Display Target

Narrative Purpose
```

---

# HDR Hierarchy

建立 HDR 控制层级。

```text
Story

↓

Lighting

↓

Color Science

↓

LUT

↓

HDR

↓

Display
```

HDR 永远服从：

故事。

---

# HDR Profiles

统一分类。

```yaml
Cinema HDR

Streaming HDR

Television HDR

Mobile HDR

Game HDR

AI HDR

Archive HDR
```

不同平台。

独立适配。

---

# Dynamic Range Strategy

统一动态范围。

```yaml
Standard

Wide

Extended

Extreme

Custom
```

根据影片风格自动匹配。

---

# Highlight Management

统一高光策略。

```yaml
Natural Highlight

Filmic Highlight

Specular Highlight

Sun Highlight

Practical Highlight
```

高光承担：

```yaml
Hope

Focus

Energy

Reality

Power
```

禁止：

高光爆炸。

---

# Shadow Management

统一暗部策略。

```yaml
Lifted Shadow

Neutral Shadow

Deep Shadow

Filmic Shadow

Crushed Shadow
```

暗部承担：

```yaml
Mystery

Fear

Isolation

Depth

Emotion
```

禁止：

暗部死黑。

---

# Midtone Strategy

统一中间调。

```yaml
Natural

Contrast Rich

Portrait

Documentary

Stylized
```

人物优先。

---

# Peak Brightness

统一峰值亮度。

```yaml
600 nits

1000 nits

2000 nits

4000 nits

Platform Adaptive
```

根据交付平台自动选择。

---

# Tone Mapping

统一 Tone Mapping。

```yaml
Filmic Curve

Perceptual

Linear

Adaptive

Custom Curve
```

保证：

HDR→SDR 一致。

---

# Local Contrast

局部反差。

统一控制。

```yaml
Low

Balanced

Enhanced

Cinematic

Extreme
```

避免：

HDR 人工痕迹。

---

# Color Volume

统一颜色体积。

```yaml
Standard

Wide

Extended

HDR Native
```

保证：

亮部颜色不丢失。

---

# Highlight Roll-off

统一高光压缩。

```yaml
Soft

Balanced

Smooth Filmic

HDR Native
```

禁止：

硬裁切。

---

# Shadow Roll-off

统一暗部过渡。

```yaml
Soft

Balanced

Deep Filmic

Adaptive
```

保证：

层次连续。

---

# Display Adaptation

适配终端。

```yaml
Cinema Projector

HDR Monitor

OLED

Mini LED

LCD

Mobile
```

统一输出逻辑。

---

# HDR Compatibility

统一兼容。

```yaml
HDR10

HDR10+

Dolby Vision

HLG

SDR
```

保证：

跨平台一致。

---

# Lighting Synchronization

HDR 同步：

```yaml
Lighting

Exposure

Reflection

Atmosphere

Practical Lights
```

确保：

光能量一致。

---

# AI HDR Constraints

针对 AI 视频。

建立：

```yaml
Stable Highlight

Stable Shadow

Stable Midtone

Stable Tone Mapping

Stable Exposure

Stable Dynamic Range
```

避免：

HDR 漂移。

---

# HDR Workflow

```text
Lighting

↓

Color Science

↓

LUT

↓

HDR Grade

↓

Tone Mapping

↓

Validation

↓

Delivery
```

不得跳步。

---

# HDR Output

统一输出。

```yaml
HDR Profile

Peak Brightness

Tone Mapping

Contrast Profile

Highlight Strategy

Shadow Strategy

Display Target

AI Constraint
```

供：

ACES Pipeline。

AI Color Constraints。

Prompt Compiler。

统一调用。

---

# Validation Rules

检查：

✓ HDR 是否符合导演意图。

✓ 高光是否自然。

✓ 暗部是否保留层次。

✓ SDR 是否一致。

✓ 是否兼容目标平台。

✓ AI 是否稳定生成。

任何失败。

禁止进入：

ACES Pipeline。

---

# Lock Rules

锁定：

```yaml
HDR Profile

Tone Mapping

Peak Brightness

Contrast Strategy

Display Target
```

允许：

后续模块补充：

```yaml
Platform Metadata

Delivery Metadata

Master Export

Archive Version
```

禁止修改：

HDR 设计逻辑。

---

# Director Notes

自动生成。

```yaml
HDR Quality

Highlight Detail

Shadow Detail

Display Consistency

Narrative Support

AI HDR Stability
```

供导演、摄影指导、调色师与DI团队审核。

---

# Final Principle

Hollywood Director OS 中。

HDR 的真正价值。

不是让观众觉得：

"画面更亮了。"

而是让观众相信：

**阳光真的耀眼。**

**火焰真的炽热。**

**黑夜真的深邃。**

HDR Workflow Engine 输出的是一套符合好莱坞真人电影工业标准，并兼容 Seedance、Veo 等 AI 视频生成模型的 HDR 工作流系统，为 ACES Pipeline、AI Color Constraints、Color Validation 与 Prompt Compiler 提供统一、稳定、跨平台一致的高动态范围影像基础。

# End of File

# Next File

Volume05 / File：07_ACES_Pipeline.md