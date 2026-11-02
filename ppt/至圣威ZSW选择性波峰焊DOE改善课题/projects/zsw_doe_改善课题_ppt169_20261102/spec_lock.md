<!-- ppt-master-schema: spec-lock/v1 -->
# Execution Lock

## canvas
- viewBox: 0 0 1280 720
- format: PPT 16:9

## communication
- primary_language: zh-CN
- audience: 品质/工艺工程师 + 质量评审委员会
- objective: 报告+说明+获取批准 — 基线32%暴露痛点 · 机理锁4因子 · DOE方案获批 · 验证标准对齐 · 量产路线明确
- core_message: ZSW 单点可编程 × L8 筛选 DOE · 多锡少锡 32% → ≤5% · 工艺从经验变成可量化窗口
- consumption_mode: presentation

## mode
- mode: custom
- mode_behavior: engineering blueprint grid alignment, KPI-first data hierarchy

## visual_style
- visual_style: data-first

## colors
- bg: #F5F7FA
- primary: #1B3A5C
- accent: #F2B84B
- text: #1E293B

## typography
- font_family: Microsoft YaHei
- title_family: Microsoft YaHei
- body_family: Microsoft YaHei
- body: 16
- title: 22

## icons
- library: inline (Office default shapes + SVG path)
- inventory: check-mark-ok · cross-bad · arrow-right · numbered-badge-01-05 · amber-warning

## page_rhythm
- P01: anchor
- P02: anchor
- P03: dense
- P04: dense
- P05: dense
- P06: dense
- P07: breathing
- P08: dense
- P09: dense
- P10: dense
- P11: dense
- P12: dense
- P13: dense
- P14: breathing
- P15: dense
- P16: anchor
- P17: dense
- P18: dense

## pptx_structure
- mode: flat

## forbidden
- `mask`, `<style>`, `class`, external CSS, `<foreignObject>`, `textPath`, `@font-face`, `<animate*>`, `<set>`, `<script>` / event attributes, `<iframe>`
- HTML named entities in text; write typography as raw Unicode and escape XML reserved characters
