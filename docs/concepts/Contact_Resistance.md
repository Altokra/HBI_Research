---
type: concept
tags:
  - concept
  - 电学特性
date_created: 2026-03-20
related_papers: [[C2W_HBI]]
---

# 接触电阻 (Contact Resistance)

> [!def] 定义 (Definition)
> 接触电阻是指两个导体接触界面处产生的附加电阻，在HBI中指Cu-Cu键合界面的电阻值。

## 📖 基本原理 (Fundamentals)

### 物理背景

接触电阻的来源：
1. **收缩电阻**：电流通过接触点时流线收缩，有效导电面积减小
2. **膜层电阻**：接触面的氧化层、污染层等产生的电阻

### 数学模型

简化的接触电阻公式：

$$
R_{contact} = \frac{\rho}{2a} + \frac{\sigma}{\pi a^2}
$$

其中：
- $\rho$ - 金属电阻率 (Ω·m)
- $a$ - 实际接触半径 (m)
- $\sigma$ - 表面膜层电阻率 (Ω·m²)

### Holm接触模型

对于多个微接触点的情况：

$$
R_{contact} = \frac{\rho}{2\sum a_i} + \frac{\rho}{2\sqrt{\pi \sum a_i^2}}
$$

## 🔗 与HBI的关系 (Relevance to HBI)

### 在混合键合中的作用

- 接触电阻直接影响信号传输损耗
- 高接触电阻会增加功耗和发热
- 是评估键合质量的关键指标

### 影响因素

| 因素 | 影响 |
|------|------|
| Cu表面氧化 | 显著增加接触电阻 |
| 键合温度 | 高温促进Cu扩散，降低电阻 |
| 键合压力 | 增加实际接触面积 |
| 表面粗糙度 | 影响接触点数量和面积 |
| 键合时间 | 影响Cu晶粒生长 |

## 📊 参数与指标 (Parameters & Metrics)

| 参数 | 符号 | 单位 | 典型值 | 说明 |
|------|------|------|--------|------|
| 接触电阻 | R_contact | mΩ | 50-200 | HBI单点接触电阻 |
| 比接触电阻 | ρ_c | Ω·μm² | - | 归一化参数 |
| Cu电阻率 | ρ_Cu | Ω·m | 1.68×10⁻⁸ | 20°C时 |

### 与Micro-bump对比

| 互连方式 | 接触电阻 | 原因 |
|----------|----------|------|
| Micro-bump | 100-300 mΩ | 存在IMC层、焊料 |
| HBI | 50-100 mΩ | 直接Cu-Cu键合 |

## 🔁 相关概念 (Related Concepts)

- [[HBI基础]] - 混合键合原理
- [[寄生参数]] - 包含接触电阻的完整模型
- [[键合工艺]] - 影响接触电阻的工艺因素

## 📚 参考文献 (References)

- [[C2W_HBI]] - 论文中报告~50mΩ的接触电阻
- R. Holm, "Electric Contacts: Theory and Applications"
