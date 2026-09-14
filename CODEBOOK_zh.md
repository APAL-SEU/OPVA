# 列说明（CSV 标注文件）

每一行是一名被试。文件：`Training.csv`（n=483）、`Validation.csv`（n=67）、`Testing.csv`（n=134）。合计 **684**。
他评 HEXACO 与职业素养为 5 点 BARS（1 = 非常低，5 = 非常高，允许一位小数）。HEXACO-60 自评为 5 点 Likert（1 = 非常不同意，5 = 非常同意）。

八道面试题各激活 Extraversion 或 Conscientiousness 的一个 **facet**。视频文件名为 `{id}_q{1-8}.mp4`，按划分放在 `Training/`、`Validation/`、`Testing/`。

## 标识与人口学信息

| 列 | 含义 | 编码 |
| --- | --- | --- |
| `id` | 被试编号（与视频文件名对应） | 字符串。多数为 24 位 Prolific 风格哈希；40 个短 ID（如 `OD66`）为滚雪球抽样被试。 |
| `gender` | 性别 | 1 男；2 女；3 非二元 / 第三性别 |
| `age` | 年龄（岁） | 连续（18–66） |
| `education` | 最高学历 | 1 高中以下（n=4）；2 高中毕业（n=55）；3 大学肄业 / 低于本科（n=183）；4 本科或同等（n=305）；5 研究生（n=137） |
| `work_experience` | 工作年限 | 连续；**2** 名训练被试缺失 |
| `job_applications` | 近两年投递次数 | 计数；**2** 名训练被试缺失（与工作年限缺失不是同一批人） |
| `english_proficiency` | 英语水平（自评） | 1 远低于平均 … 5 远高于平均。实际取值：1、3、4、5 |

## 他评外向性 / 尽责性（`p_*_observer`）

`p_X_observer` / `p_C_observer` 分别为对应四个 facet 列的平均。

| 列 | 含义 | 对应题 | 编码 |
| --- | --- | --- | --- |
| `p_X_observer` | 外向性 Extraversion（他评；四个 X facet 平均） | q1, q3, q5, q7 | 1–5 |
| `p_C_observer` | 尽责性 Conscientiousness（他评；四个 C facet 平均） | q2, q4, q6, q8 | 1–5 |
| `p_Xsses_observer` | 社会自尊 Social self-esteem | q1 | 1–5 |
| `p_Xsbol_observer` | 社交大胆 Social boldness | q3 | 1–5 |
| `p_Xsoci_observer` | 社交性 Sociability | q5 | 1–5 |
| `p_Xlive_observer` | 活力 Liveliness | q7 | 1–5 |
| `p_Corga_observer` | 条理性 Organization | q2 | 1–5 |
| `p_Cdili_observer` | 勤奋 Diligence | q4 | 1–5 |
| `p_Cperf_observer` | 完美主义 Perfectionism | q6 | 1–5 |
| `p_Cprud_observer` | 审慎 Prudence | q8 | 1–5 |

## 自评 HEXACO（`*_self`）

HEXACO-60：每个因子 10 题，因子分 = 10 道（已反向）题目的平均。

| 列 | 含义 | 编码 |
| --- | --- | --- |
| `H_self` | 诚实-谦逊 Honesty-Humility（自评） | 1–5 |
| `E_self` | 情绪性 Emotionality（自评） | 1–5 |
| `X_self` | 外向性 Extraversion（自评） | 1–5 |
| `A_self` | 宜人性 Agreeableness（自评） | 1–5 |
| `C_self` | 尽责性 Conscientiousness（自评） | 1–5 |
| `O_self` | 开放性 Openness to Experience（自评） | 1–5 |

## 他评职业素养（`mean_rating_*`）

两名职业招聘官评分的平均。

| 列 | 含义 | 编码 |
| --- | --- | --- |
| `mean_rating_dev_orient` | 发展导向 Development orientation：投入学习以拓宽技能、专业成长 | 1–5 |
| `mean_rating_com_flex` | 沟通灵活 Communication flexibility：按对象调整表达方式 | 1–5 |
| `mean_rating_persuasiveness` | 说服力 Persuasiveness：用论据、权威和/或策略争取认同 | 1–5 |
| `mean_rating_qual_orient` | 质量导向 Quality orientation：努力达到或超过质量标准 | 1–5 |
| `mean_rating_hirea` | 整体录用潜力（针对管理培训生岗位） | 1–5 |

## 划分

| 划分 | n | 标注文件 | 视频目录 |
| --- | --- | --- | --- |
| train | 483 | `Training.csv` | `Training/` |
| validation | 67 | `Validation.csv` | `Validation/` |
| test | 134 | `Testing.csv` | `Testing/` |
