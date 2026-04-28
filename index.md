---
title: 电信客户流失生存分析报告
---

# 电信客户流失生存分析报告

欢迎访问我的数据分析博客！

本报告基于公开数据集 **`WA_Fn-UseC_-Telco-Customer-Churn.csv`**，对电信客户的流失行为进行深入的**生存分析（Survival Analysis）**。通过整合四种主流方法，全面刻画客户生命周期特征，并为业务决策提供量化依据。

## 分析方法概览

本项目综合运用了以下四类生存分析技术：

- **Kaplan-Meier 非参数估计**：可视化不同客户群体（如是否签订长期合约、是否使用光纤网络等）的留存概率随时间的变化趋势。
- **Cox 比例风险模型（Cox Proportional Hazards Model）**：识别影响客户流失风险的关键协变量（如月费、服务类型、付款方式等），并评估其风险比（Hazard Ratio）。
- **加速失效时间模型（Accelerated Failure Time, AFT）**：在假设特定生存分布（如Weibull或Log-Normal）下，直接建模客户生命周期的尺度效应，提供更直观的时间解释。
- **客户生命周期价值（Customer Lifetime Value, CLV）估算**：结合生存预测与历史消费数据，量化高价值客户的预期贡献，辅助精准营销与挽留策略制定。

## 报告内容

- 数据清洗与特征工程
- 生存时间与事件变量的定义
- Kaplan-Meier 曲线与 Log-rank 检验结果
- Cox 模型拟合诊断与变量显著性
- AFT 模型选择与参数解释
- CLV 计算逻辑与分群洞察
- 业务建议：如何降低流失率、提升客户留存

> 本博客完整记录了从数据探索到模型部署的全流程，所有代码均开源，旨在分享可复现的分析实践。

---

*数据来源：IBM Sample Dataset - Telco Customer Churn*  
*分析工具：Python (lifelines, scikit-learn, pandas, matplotlib)*
