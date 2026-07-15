# 电商平台用户行为分析与 RFM 价值分层体系搭建

## 项目简介
本项目基于电商平台用户行为与属性数据，完成数据清洗、用户画像分析、消费行为分析与 RFM 用户价值分层，为精细化运营提供数据支撑。

当前数据集已由原始 1,000 条扩展为 80,000 条用户样本，覆盖用户属性、行为特征、消费价值三类字段。

## 分析流程
1. 数据读取与基础清洗
2. 用户性别、年龄、地域、兴趣画像分析
3. 用户活跃度与订阅行为分析
4. 产品品类偏好与年龄层消费分析
5. RFM 用户价值分层
6. 用户总消费相关性分析

## 技术栈
- Python
- Pandas、NumPy
- Matplotlib、Seaborn
- SciPy
- RFM 用户分层模型

## 文件说明
- `data/user_personalized_features.csv`：80,000 条用户行为数据
- `data/user_personalized_features_backup_1000.csv`：原始 1,000 条数据备份
- `rfm_analysis_80k.py`：本地可直接运行的 80,000 条数据分析代码
- `notebooks/电商平台用户行为分析与 RFM 价值分层体系搭建.ipynb`：Notebook 分析版本
- `imgaes/`：分析过程中生成的可视化图表
- `requirements.txt`：项目运行依赖

## 如何运行
在项目根目录执行：

```bash
pip install -r requirements.txt
python rfm_analysis_80k.py
```

运行完成后，终端会输出数据清洗结果、RFM 用户分层结果和相关性分析结果，图表会保存到 `imgaes/` 目录。

## 数据说明
主要字段包括：

- 用户属性：`User_ID`、`Age`、`Gender`、`Location`、`Income`、`Interests`
- 行为特征：`Last_Login_Days_Ago`、`Time_Spent_on_Site_Minutes`、`Pages_Viewed`、`Newsletter_Subscription`
- 消费特征：`Purchase_Frequency`、`Average_Order_Value`、`Total_Spending`、`Product_Category_Preference`

## 运行结果概览
当前 80,000 条数据运行后的 RFM 分层结果为：

| 用户分层 | 用户数量 |
| --- | ---: |
| 低价值用户 | 16,696 |
| 新用户 | 12,529 |
| 流失高价值用户 | 11,694 |
| 需召回用户 | 11,422 |
| 流失预警用户 | 8,188 |
| 潜力用户 | 7,353 |
| 深耕用户 | 7,081 |
| 高价值用户 | 5,037 |

