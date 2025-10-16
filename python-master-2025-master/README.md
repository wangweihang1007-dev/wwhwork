# Python 金融数据分析（专硕 2025）

面向金融学专业硕士的 Python 实战课程仓库。包含 14 节核心课件（Jupyter Notebooks）、教学用数据集与可视化素材，覆盖从数据导入、收益计算、可视化，到投资组合、CAPM、Fama‑French 因子与市场异象等主题。

---

## 课程目录（Notebooks）

按建议学习顺序列出主要课件与主题：

1. `Class 01 Import Data.ipynb`：金融数据导入与基础清洗
2. `Class 02 Calculate Return.ipynb`：收益率计算（按日/按月等）
3. `Class 03 Return Picture.ipynb`：收益率可视化（时间序列、分布等）
4. `Class 04 Summary.ipynb`：描述统计与探索性数据分析（EDA）
5. `Class 05 Hypothesis Testing.ipynb`：假设检验（t 检验、正态性等）
6. `Class 06 Predict Return.ipynb`：收益率预测的基本回归框架
7. `Class 07 Predict Return volatility.ipynb`：波动率预测
8. `Class 08 Predict Return Volume.ipynb`：成交量与收益的预测关系
9. `Class 09 Price Ratio.ipynb`：价格比率与均值回归思路
10. `Class 10 Portfolio.ipynb`：投资组合构建与绩效评估
11. `Class 11 CAPM.ipynb`：资本资产定价模型（CAPM）
12. `Class 12 Size and Value Portfolio.ipynb`：规模与价值组合（SMB/HML 思想）
13. `Class 13 Fama-French 3 Factors.ipynb`：Fama‑French 三因子模型
14. `Class 14 Anomalies.ipynb`：市场异象与横截面检验

补充课件：
- `Class OLS .ipynb`：普通最小二乘（OLS）回归要点
- `Class Out-of-Sample.ipynb`：样本外检验与滚动预测
- `点名.ipynb`：课堂点名使用，可忽略

---

## 数据与素材

教学数据均用于课程演示与练习，常见文件如下（非穷尽）：

- `datasets/TRD_Cnmont.xlsx`：A 股月度收益示例
- `datasets/Marketret_mon_stock2023.xlsx`：市场收益率示例
- `datasets/ret_mon_python2023.csv`：月度收益示例
- `datasets/cross_section.csv`、`datasets/cross_section2023.csv`：横截面因子/收益示例
- `datasets/rolling_betas.csv`：滚动 Beta 示例
- `datasets/inflation.csv`：通胀（CPI）示例
- `datasets/US stock market return.csv`：美国股市收益示例
- `datasets/Turnover_individual_mon2022.csv`：个股换手率示例
- `datasets/EP2023.csv`：盈利/价格比（E/P）示例
- `datasets/priceratio.csv`：价格比率示例
- `datasets/000001.csv`、`datasets/Block.csv` 等：个股/交易特征示例

可视化素材位于 `images/`，包含课程配图与演示图片。

提示：不同数据来源口径可能存在差异，仅用于教学与方法演示，非投资建议。

---

## 常见问题（FAQ）

- 读取 Excel 报错：请确认已安装 `openpyxl` 或 `xlrd`（见上文安装命令）。
- 中文显示异常：Matplotlib 可能需要设置中文字体，可在 Notebook 中手动配置字体。
- 日期解析：使用 `pd.to_datetime` 并留意格式（如是否为月度收盘日期）。
- 路径问题：确保在仓库根目录启动 Jupyter，或在 Notebook 中调整相对路径为 `datasets/...`。
- 结果可复现性：涉及随机过程时可设置随机种子，例如 `np.random.seed(42)`。

---

## 仓库结构

```
.
├── Class 01 ... 14 *.ipynb        # 课程主线 Notebook
├── Class OLS .ipynb               # OLS 补充
├── Class Out-of-Sample.ipynb      # 样本外检验补充
├── datasets/                      # 教学数据（CSV/XLSX 等）
├── images/                        # 课程图片与素材
├── README.md                      # 本文件（中文）
└── README.en.md                   # 英文说明
```

---

## 贡献与反馈

- 欢迎通过 Issues/Pull Requests 提交勘误、改进建议或补充案例。
- 贡献时请尽量：
  - 保持 Notebook 可复现实验（相对路径、固定随机种子等）。
  - 统一风格与术语，便于教学。

---

## 许可协议

本项目采用 MIT License，允许在遵守协议的前提下自由使用与修改代码。若需要正式许可文件，可在仓库中添加标准 `LICENSE` 文件。

---

## 致谢

感谢课程助教与同学的使用与反馈，祝学习顺利！
