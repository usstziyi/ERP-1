# EEG预处理与ERP/时频分析学习计划

## 学习计划概述

本计划系统、循序渐进地讲解EEG（脑电图）预处理技术，重点涵盖**ERP（事件相关电位）**和**时频分析**两大核心分析方法。整个学习路径分为5个逻辑连贯的单元，从基础概念逐步过渡到高级分析方法，最终通过mne-sample-data数据集完成完整的EEG数据处理与分析流程。

---

## 学习单元结构

| 单元 | 主题 | 内容 |
|------|------|------|
| **Unit 1** | EEG基础与MNE数据结构 | EEG信号基础、MNE-Python核心数据结构、数据加载与可视化 |
| **Unit 2** | EEG预处理基础操作 | 滤波、重参考、坏道检测与插值、ICA去伪迹、Epoch提取 |
| **Unit 3** | ERP分析原理与实现 | ERP理论基础、平均ERP计算、组件识别、统计分析与可视化 |
| **Unit 4** | 时频分析方法与应用 | 时频分解原理、小波变换、FFT谱分析、ERS/ERD计算 |
| **Unit 5** | 综合案例分析 | 使用mne-sample-data完成从原始数据到ERP/时频分析的完整流程 |

---

## 环境依赖

| 库名称 | 版本号 | 用途 |
|--------|--------|------|
| Python | >=3.9 | 核心编程语言 |
| mne | >=1.6.0 | EEG/MEG数据处理核心库 |
| numpy | >=1.24.0 | 数值计算 |
| scipy | >=1.10.0 | 科学计算与信号处理 |
| matplotlib | >=3.7.0 | 数据可视化 |
| pandas | >=2.0.0 | 数据管理与统计 |
| jupyter | >=1.0.0 | Notebook运行环境 |
| mne-bids | >=0.14.0 | BIDS格式数据处理 |
| autoreject | >=0.4.0 | 自动伪迹拒绝 |

---

## 学习建议

1. **按顺序学习**：每个单元建立在前一单元的基础之上，建议按顺序完成
2. **理论+实践**：每个单元包含理论讲解和配套代码，建议先理解理论后再运行代码
3. **动手修改**：鼓励修改代码中的参数，观察不同参数对结果的影响
4. **记录问题**：在学习过程中记录疑问，便于后续深入探究
5. **参考文档**：建议配合[MNE-Python官方文档](https://mne.tools/stable/index.html)学习

---

## 数据集说明

最终单元（Unit 5）使用 **mne-sample-data** 数据集，该数据集包含：
- 一名受试者的MEG/EEG联合记录
- 听觉和视觉诱发的实验范式
- 包含结构MRI数据
- 适合演示完整的EEG预处理和分析流程

---

## 输出文件说明

每个单元包含一个Jupyter Notebook文件（`.ipynb`格式），文件命名规则：
- `Unit_01_EEG_Basics_and_MNE_Structure.ipynb`
- `Unit_02_EEG_Preprocessing_Basics.ipynb`
- `Unit_03_ERP_Analysis.ipynb`
- `Unit_04_Time_Frequency_Analysis.ipynb`
- `Unit_05_Complete_Workflow_with_mne_sample_data.ipynb`
