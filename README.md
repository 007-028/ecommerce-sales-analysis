# 电商平台用户行为分析与RFM价值分层

## 项目简介
基于电商用户行为数据集，通过数据清洗、探索性分析与RFM用户分层模型，挖掘用户行为特征与价值分布，为精细化运营提供数据支撑。

## 分析流程
1. 数据清洗与预处理
2. 用户行为多维度探索分析
3. RFM用户价值分层模型搭建
4. 结论与运营优化建议

## 技术栈
- Python (Pandas, NumPy)
- 数据可视化：Matplotlib, Seaborn
- 分析方法：RFM用户分层、多维度拆解

## 文件说明
- `notebooks/ecommerce_rfm_analysis.ipynb`：完整分析代码与报告
- `data/user_behavior.csv`：原始数据集
- `images/`：分析过程中生成的可视化图表

## 如何运行
```bash
# 安装依赖
pip install -r requirements.txt

# 启动Jupyter Notebook
jupyter notebook notebooks/ecommerce_rfm_analysis.ipynb
