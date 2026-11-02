<!-- ppt-master-schema: design-spec/v1 -->
# zsw_doe_改善课题 - Design Spec

## I. Project Information

| Item | Value |
| --- | --- |
| Project Name | zsw_doe_改善课题 |
| Canvas Format | PPT 16:9 (1280×720) |
| Page Count | 18 |
| Target Audience | 品质/工艺工程师 + 质量评审委员会（懂统计、懂生产工艺，关心良率和工艺稳定性） |
| Communication Intent | 报告并说明改善现状与机理（report），解释为什么选这 4 个因子，汇报 DOE 方案（explain），获得评审委员会批准执行资源（decide） |
| Desired Audience Outcome | 评审通过 DOE 执行资源 · 认识 ZSW 局部调参价值 · 承诺严格按 RunOrder 执行 8 组实验 |
| Core Message / Ask / Action | ZSW 单点可编程 × L8 筛选 DOE · 多锡少锡 32% → ≤5% · 工艺从经验变成可量化窗口 |
| Delivery Context | 主 presenter-led 会议室投影；次要后续实验方案 hand-off + 验证结果汇报 + 量产试产 |
| Artifact Afterlife | 评审 archive + 执行团队 hand-off + Minitab 数据回填 + 量产试产对比依据 |
| Reading Mode | presentation — 每页一个核心 claim + 大数字 + 关键词短语，细节进 speaker notes |
| Content Strategy | stay close — 严格跟踪 source 10 章节结构与定量数据（32%, L8(2⁴), t=2.06, α=0.05, RunOrder 随机化, 4 因子 A/B/C/D），仅将长段落压缩为 presentation 短语 |
| Design Style | Engineering Blueprint · Grid mode + data-first visual style + scientific rendering |
| AI Image Acquisition Path | placeholder only — 第 4 页 PCB 不良实拍待实验前补，其余页面无 AI 图需求 |
| Generation Mode | continuous |
| Spec Refinement | disabled |
| Speaker Notes | enabled — 每页配演讲者备注（proactive Stage-2 policy） |
| Custom Animations | disabled — 答辩场景不需过场动画（proactive Stage-2 policy） |
| Narration Audio | disabled — 无明确需求（proactive Stage-2 default） |
| Created Date | 2026-11-02 |

## II. Canvas Specification

| Property | Value |
| --- | --- |
| Format | PPT 16:9 |
| Dimensions | 1280×720 |
| viewBox | `0 0 1280 720` |
| Margins | 40 px left/right, 32 px top/bottom |
| Content Area | 40..1240 × 32..688 |

## III. Visual Theme

### Theme Style

- **Mode**: grid — 结构化工程蓝图感，网格对齐每一节
- **Visual style**: data-first — KPI 大数字先行，图表和表格承载数据，文字精炼
- **Theme**: engineering-blueprint — 深蓝主色 + 钢蓝次色 + 琥珀强调 + 湖青点缀
- **Tone**: authoritative + precise + process-oriented

### Color Scheme

| Role | HEX | Purpose |
| --- | --- | --- |
| Background | #F5F7FA | 冷灰底，降低长时间观看疲劳 |
| Secondary background | #FFFFFF | 卡片、表格底色 |
| Primary | #1B3A5C | 深蓝：标题、章节标签、大数字、header band |
| Accent | #F2B84B | 琥珀：KPI、警示、高亮、风险 flag |
| Secondary | #17A2B8 | 湖青：标签、勾选、正向强调 |
| Body text | #1E293B | 正文深灰 |
| Text secondary | #475569 | 次要文本 |
| Text tertiary | #94A3B8 | 注释/页码 |
| Divider | #E2E8F0 | 分割线/表格边框 |
| Bad | #DC2626 | 风险框/不良率 |
| Ok | #16A34A | 目标达成/成功 |

## IV. Typography System

### Font Plan

| Role | Character (Reference) | Primary | English if non-English | Fallback tail |
| --- | --- | --- | --- | --- |
| Title | CJK | Microsoft YaHei | Arial | sans-serif |
| Body | CJK | Microsoft YaHei | Arial | sans-serif |

- **Title stack**: "Microsoft YaHei", "PingFang SC", Arial, sans-serif
- **Body stack**: "Microsoft YaHei", Arial, sans-serif

### Font Size Hierarchy

| Purpose | Size (px) |
| --- | --- |
| Body | 16 |
| Page title | 22 |
| Subtitle | 12-13 |
| Annotation | 11 |
| Footnote | 10 |

## V. Layout Principles

### Deck-wide Direction

- **Hierarchy direction**: top-down, section band → content zone → footer band; primary nav through left-to-right labels (Chapter tag + title)
- **Composition tendency**: equal-weight card grid for TOC, dominant KPI + side-labels for data pages, two-column split for problem/advantage pages, centered hero for cover and conclusion
- **Cross-page continuity**: Accent-colored chapter tag in header repeats page role across 18 pages (e.g. "01 · 项目背景" for P03-P04)
- **Spacing posture**: loose enough for breathing on anchor pages (cover, TOC, conclusion); tight + dense on table/chart pages

## VI. Icon Usage Specification

| Icon Path | Suitable Scenarios |
| --- | --- |
| ✓ Secondary #17A2B8 | ✅ 入选 DOE 因子 |
| ✗ Bad #DC2626 | ❌ 固定噪声因子 |
| → Accent arrow | 下一步 / 流程 step |
| 01-05 Primary circle badge | section / risk numbered steps |
| ! Amber triangle | 风险 flag / 备注 |

## VII. Visualization Reference

| Visual | Page | Construction |
| --- | --- | --- |
| KPI big number box | P01, P03 | native textbox + Primary #1B3A5C fill · Amber 64px number centered |
| DOE L8 正交表 | P09 | native pptx table · Primary header · alternating row stripes |
| 5M1E analysis table | P05 | native pptx table · ✅/❌ checkmark cells |
| Process comparison table | P06 | native pptx table · Primary header + NAVY conclusion bar below |
| Pareto bar chart | P11 | native chart column type + Secondary bars + red α=0.05 threshold line overlay |
| Main effects line charts (2×2 grid) | P12 | native chart line type × 4 subcharts |
| Step flow cards | P10, P13, P14 | step number badge + label + description |
| Q&A card | P18 | circle Q icon + bold question + regular answer |

## VIII. Image Resource List

| Filename | Dimensions | Ratio | Purpose | Type | Image pattern | Crop Policy | Acquire Via | Status | Reference | text_policy | page_role |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| p04_pcb_多锡_placeholder | 420×230 | 16:9 | 证据图 | user photo | placeholder | center-crop | placeholder (user) | Needs-Manual | placeholder block | overlay-caption | evidence-photo |
| p04_pcb_少锡_placeholder | 420×230 | 16:9 | 证据图 | user photo | placeholder | center-crop | placeholder (user) | Needs-Manual | placeholder block | overlay-caption | evidence-photo |
| pareto_data_p11 | 800×450 | 16:9 | 数据驱动图 | scenario chart | none | native | scenario | Generated | A=5.2,B=4.1,C=1.3,D=0.7 | none | data-chart |
| main_effects_data_p12 | 800×450 | 16:9 | 数据驱动图 | scenario chart | none | native | scenario | Generated | A=[70,32],B=[68,34],C=[48,52],D=[46,54] | none | data-chart |

## IX. Content Outline

### Part 1: 封面 · TOC · 项目背景

#### Slide 01 - 封面 · anchor · cover impact
- **Audience move**: 第一眼被 32% 琥珀大数字抓住；立即意识到课题严重性；副标题说明是 DOE + Minitab 工程报告
- **Composition**: Primary #1B3A5C 深蓝整幅底 + Accent #17A2B8 左侧装饰竖条 + hero title 居中偏左 + 底部 info band
- **Title**: 至圣威 ZSW 选择性波峰焊 · 局部焊点多锡/少锡不良改善 DOE 课题
- **Core message**: 32% 基线不良率是起点
- **Content**: hero title + subtitle + 32% Amber 64px + 部门/姓名/日期底部 band
- **Relationships**: none

#### Slide 02 - 目录 · anchor
- **Audience move**: 7 章节快速扫过，建立完整路线认知
- **Composition**: 黑白条纹交替 7 行卡片列表 · 序号标签 + 标题 + 一句话描述
- **Title**: 目 录 · CONTENTS
- **Content**: 7 章节（01-07）· 每行序号 Primary · 标题 bold · 描述 muted
- **Relationships**: none

#### Slide 03 - 项目背景 · dense
- **Audience move**: KPI 32% box 先行 → 逐条理解痛点 → 最后被课题目标号召
- **Composition**: 左 320px KPI box · 右 4 个要点标签卡 vertical stack
- **Title**: 项目背景：为什么要开展本课题
- **Content**: 现状描述 · 原有方式 · 设备基础 · 课题目标（Goal Accent tag）
- **Relationships**: none

#### Slide 04 - 问题描述 · dense
- **Audience move**: 左图 placeholders 建立视觉预期 → 右要点理解现象和风险 → 基线数据锚定
- **Composition**: 左 2 张 420×230 placeholder photo blocks + 右要点列 + 基线 KPI 小框
- **Title**: 问题描述：不良现象实拍
- **Content**: 不良现象 3 条 · 质量风险 2 条 · 基线数据 32%

### Part 2: 机理分析 · 工艺对比 · DOE 目标

- **Relationships**: contrast (多锡堆锡 vs 少锡不足)
#### Slide 05 - 机理分析 · dense
- **Audience move**: 5M1E 表格一行行扫过 → 看到 4 个 ✅ 入选和 2 个 ❌ 固定 → 理解为什么选这 4 个
- **Composition**: Primary header table · 黑白条纹 · ✅/❌ 标记 cell
- **Title**: 不良机理分析 · 5M1E 简化版
- **Content**: 维度 · 潜在根因 · 是否纳入 DOE · 备注（7 行 4 列）
- **Relationships**: membership (4 入选 vs 2 固定)

#### Slide 06 - 工艺对比 · dense
- **Audience move**: 6 维度横向对比 → 看到 ZSW 比传统多出的 3 个可编程独立调参 → 认同是典型应用场景
- **Composition**: Primary header table + NAVY conclusion bar below
- **Title**: ZSW 选择性波峰焊 vs 传统波峰焊
- **Content**: 焊接方式 / 助焊剂 / 走速 / 浸锡 / 脱锡 / 局部优化（7 行 3 列）
- **Relationships**: contrast (传统 vs ZSW 六维度)

#### Slide 07 - DOE 目标 · breathing
- **Audience move**: 4 个动词方卡（识别/寻找/建立/验证）快速扫过 → Y1 望小 + Y2 望大双响应框 · 理解实验目的
- **Composition**: 4 个 horizontal stacked step cards · 底部 BAD 框 Y1 + OK 框 Y2 并列
- **Title**: DOE 实验目标 · Y 双响应
- **Content**: 4 项目标 · Y1 不良率 % 望小 · Y2 锡量评分 1-5 望大
- **Relationships**: membership (4 项目标 + 2 响应指标 Y1/Y2)

#### Slide 08 - 因子与水平 · dense
- **Audience move**: A/B/C/D 四因子 · -1/+1 水平拉开差异 · 理解每个因子为什么这样设定
- **Composition**: Primary header table · 下方 Amber principle note band
- **Title**: 因子与水平选定 · 4 因子 2 水平
- **Content**: A 助焊剂喷涂量 · B 熔锡池走速 · C 浸锡停留时间 · D 脱锡方向补偿（5 行 5 列）

### Part 3: L8 设计 · 执行计划 · Minitab 分析

- **Relationships**: membership (A/B/C/D 四因子并列)
#### Slide 09 - L8 正交表 · dense
- **Audience move**: 8 组 RunOrder 随机化表 → 理解为什么 RunOrder 而非 StdOrder
- **Composition**: Primary header table + 下方 Minitab configuration note band
- **Title**: L8(2⁴) 筛选 DOE 正交表
- **Content**: RunOrder/StdOrder/A/B/C/D/Y1/Y2（10 行 7 列）
- **Mathematical content**: t threshold 2.06 at α 0.05 (intended for P11 chart threshold)
- **Relationships**: order (RunOrder 1→8 随机化)

#### Slide 10 - 执行计划 · dense
- **Audience move**: 5 个 step cards · 理解样品量/噪声/物料/判定/数据 5 条 checklist
- **Composition**: 5 个 horizontal stacked cards + bottom amber note
- **Title**: 上机实验执行管控要点
- **Content**: 样品量 ≥2拼板16pcs · 噪声锁定 · 同一批次物料 · 固定检验员 · RunOrder 上机
- **Relationships**: sequence (5 条执行 checklist)

#### Slide 11 - 帕累托图 · dense
- **Audience move**: 4 柱 + α=0.05 红虚线 · A/B 超过红线显著 · C/D 不显著
- **Composition**: 左侧 7.5×4.5 chart area · 右侧判读说明 card
- **Title**: Minitab 分析 · 标准化效应帕累托图
- **Content**: 柱 A=5.2,B=4.1,C=1.3,D=0.7 + 红线 t=2.06
- **Mathematical content**: t_critical 2.06; alpha 0.05
- **Relationships**: order (效应大小排序 A>B>C>D)

#### Slide 12 - 主效应图 · dense
- **Audience move**: 2×2 小图矩阵 → A/B 斜率显著 · C/D 斜率近水平
- **Composition**: 2×2 subchart grid · 底部 NAVY interpretation band
- **Title**: Minitab 分析 · 主效应图
- **Content**: A/B effect lines steep · C/D near horizontal

### Part 4: 最优参数 · 验证 · 收益 · 总结

- **Relationships**: contrast (显著 A/B vs 不显著 C/D)
#### Slide 13 - 最优参数推导 · dense
- **Audience move**: 4 步流程方卡 → 推荐参数表（待实验回填）
- **Composition**: 4 horizontal stacked step cards + bottom Primary recommendation table
- **Title**: 最优工艺参数组合推导
- **Content**: Step1 P筛选 → Step2 最优水平 → Step3 不显著因子 → Step4 Minitab 预测（4 行 4 列参数表）
- **Relationships**: sequence (Step 1→4 参数推导流程)

#### Slide 14 - 验证实验 · breathing
- **Audience move**: 左 5 步流程图 → 右 OK 框 4 项结案标准
- **Composition**: left flow cards + right bordered OK card (4 criteria)
- **Title**: 最优参数验证 · 必须执行不可省略
- **Content**: 3 次独立重复 · 实测 vs 预测 · 连续稳定 · 双响应达标
- **Relationships**: sequence (验证 5 步流程)

#### Slide 15 - 预期收益 · dense
- **Audience move**: 三栏并排 · 收益 ✅ · 风险 ⚠️ · RSM 进阶 📌
- **Composition**: 3 equal-width columns with colored header bands (Ok / Amber / Accent)
- **Title**: 预期收益 · 风险提示 · 进阶方案
- **Content**: 收益 4 条 · 风险 4 条 · RSM 进阶 4 条
- **Relationships**: contrast (收益 ✅ vs 风险 ⚠️)

#### Slide 16 - 总结 · anchor
- **Audience move**: hero "核心价值=局部独立微调 × DOE 工艺窗口" → 5 条编号 takeaway → 封底一句话
- **Composition**: Primary deep-blue fill · Amber hero title · 5 numbered takeaway rows · footer band
- **Title**: 课题价值总结
- **Content**: 5 takeaways + 封底一句话
- **Relationships**: membership (5 条 takeaway)

#### Slide 17 - 风险清单 · dense
- **Audience move**: 10 条风险 + 应对预案 · 逐条扫过理解答辩准备充分
- **Composition**: Primary header table · alternating rows
- **Title**: 附录 1 · DOE 方案假设与潜在风险
- **Content**: #/风险描述/潜在影响/答辩应对预案（11 行 4 列）
- **Relationships**: membership (10 条风险清单)

#### Slide 18 - Q&A · dense
- **Audience move**: 8 组 Q&A cards · 答辩预判
- **Composition**: 8 alternating stripe Q&A card rows · each with Q icon + bold question + regular answer
- **Title**: 附录 2 · 评审预判 Q&A
- **Content**: 8 Q&A pairs + bottom quote bar
- **Relationships**: none

## X. Speaker Notes Requirements

- **Generation**: enabled
- **Filename**: match each SVG filename under `notes/`
- **Content**: 每页 speaker notes 承载：
  - 统计术语解释（α=0.05, t=2.06, 随机化 RunOrder 为什么重要 · StdOrder 为什么危险）
  - 参数选择依据（为什么 A 助焊剂可能显著 · 为什么 C 不显著也不代表没用 · 为什么水平区间要先小试）
  - 工厂执行注意事项（噪声因子锁定清单 · 禁止 StdOrder · 压缩实验时长抵消时间漂移）
  - 风险应对预案（10 条风险的口头版，不是书面表格）
  - 评审可能追问预判（8 条 Q&A 的口头版本，精简回答要点）
  - 演讲过渡语（"上一页讲的是 X，下面我们看 Y"）
  Notes 深度覆盖 source 全文细节，但保持口语化简洁 · 每个 slide notes ≥ 80 字
