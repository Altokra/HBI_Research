---
type: paper
title: C2W Hybrid Bonding Interconnect Technology for Higher Density and Better Thermal Dissipation of High Bandwidth Memory
authors: Kibum Kim, Sanghyun Lee, Jinhyun Kim, et al.
year: "2023"
journal_conference: ECTC 2023
doi:
url:
tags:
  - paper/reading
  - HBI/C2W
  - HBM
status: 🟨 阅读中
rating: ⭐⭐⭐
date_created: 2026-03-17
learning_level: 工艺基础
pdf: "[[C2W_Hybrid_Bonding_Interconnect_Technology_for_Higher_Density_and_Better_Thermal_Dissipation_of_High_Bandwidth_Memory-dual.pdf]]"
---

> [!abstract] 一句话总结 (One-Sentence Summary)
> 提出了一种应用于HBM的C2W混合键合技术，相比传统micro-bump实现了更高密度互连和更好的热耗散性能。

## 💡 1. 研究背景与动机 (Motivation)

- **核心问题**：
  - AI、物联网、机器学习等高性能计算需求推动HBM发展
  - 传统micro-bump互连在pitch缩小到极限时面临挑战
  - 高功耗HBM的热管理问题日益严峻

- **作者目标**：
  - 将C2W混合键合技术应用于HBM堆叠
  - 实现比micro-bump更高的I/O密度
  - 改善热耗散性能

## 🛠️ 2. 核心创新点与方法 (Methodology)

- **键合类型**：C2W (Chip-to-Wafer)
- **键合工艺**：Cu-Cu混合键合 (Hybrid Bonding)
- **关键参数**：

| 参数                  | 数值      | 单位  |
| ------------------- | ------- | --- |
| Pitch               | 10      | μm  |
| Contact Resistance  | ~50     | mΩ  |
| Bonding Temperature | 250-300 | °C  |

### 2.1 技术优势

1. **更高互连密度**：10μm pitch vs 传统micro-bump的40-50μm
2. **更低接触电阻**：无IMC层，直接Cu-Cu键合
3. **更好热性能**：无焊料凸点，热阻更低

## 📊 3. 实验与结果 (Experiments & Results)

### 3.1 电学特性 (Electrical Characteristics)

- **接触电阻**：~50 $m\Omega$ per bump
- **寄生电容**：较micro-bump降低（无焊料凸点）
- **寄生电感**：更短的互连路径，电感更小
- **RC延迟**：整体改善

### 3.2 信号完整性 (Signal Integrity)

- **S参数**：S21在高速信号下表现良好
- **眼图**：在高速数据传输下眼图张开度良好
- **串扰**：pitch缩小后需要关注

### 3.3 热性能 (Thermal Performance)

- **热阻降低**：相比micro-bump降低约X%
- **热耗散路径**：Cu-Cu直接接触，热传导更高效

### 3.4 对比分析

| 指标 | 本工作 (HB) | Micro-bump | 改善 |
|------|-------------|------------|------|
| Pitch (μm) | 10 | 40-50 | 4-5x |
| R_contact (mΩ) | ~50 | ~100-200 | 2-4x |
| 热阻 | 更低 | 基准 | - |

### 3.5 可靠性测试

- 高温存储 (HTS)
- 温度循环 (TC)
- 高温高湿 (HTHH)

## ⚠️ 4. 局限性 (Limitations)

- 作者自己承认的局限性：
  - C2W工艺对准精度要求高
  - 良率控制挑战

- 我认为的不足之处：
  - 未详细讨论超高速信号(>10Gbps)的SI分析
  - PI分析较少涉及
  - 串扰分析不够深入

## 🧠 5. 我的思考与启发 (Takeaways)

> [!idea] 对我的启发
> - 这篇论文帮助我理解了C2W混合键合在HBM中的应用
> - 学到了关键参数：10μm pitch, ~50mΩ接触电阻
> - 下一步：了解HBI的基本原理，对比C2W与W2W的优缺点

## 🔗 6. 相关链接 (Links)

- **前置知识**：[[HBI基础]], [[C2W_vs_W2W]]
- **相关概念**：[[接触电阻]], [[寄生参数]], [[热阻]]
- **参考文献**：
  - 
- **代码仓库**：
