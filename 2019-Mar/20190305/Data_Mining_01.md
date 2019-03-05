# Part 1 Introduction

## Why Data Mining?

- 数据量庞大——数据源膨胀，存储介质廉价，互联网发展
- 大量数据中，冗余数据与脏数据多
- **We are drowning in data, but starving for knowledge!**
- 需求促进发明——数据挖掘技术：**自动**分析**大量**数据集

## What Is Data Mining?

- KDD: knowledge discovery from data.
- 从大量数据中，获取有趣的模式和知识。
  - 有趣的：非平凡的，隐式的，前所未知的，完全可理解的，正确的，潜在有用的。
  - **非平凡的(non-trivial)**: Needing significant computing power to solve.

---

KDD过程：数据库系统和数据仓库社区(?)视角：

数据库--数据清洗、数据集成--->数据仓库--数据选择-->任务相关数据--数据挖掘-->模式评估-->结果展示(可视化等)-->知识&模式&信息

*??模式：分类、聚集等*

---

## Multi-Dimension View of Data Mining

数据挖掘对象：

- 数据库(ER，OO，异构，过时)，数据仓库，事务(transaction)数据，流数据，时间序列，多媒体，等各式各样的数据形式

要挖掘的知识(挖掘目标)

- 特征

- 区别

- 关联

- 分类

- 聚集

- 趋势/方差

  ---

- 描述性 & 预测性

使用的方法

- 数据密集——Data-intensive
- 数据仓库与联机分析处理(OLAP)
- 机器学习
- 统计方法
- 模式识别
- 可视化
- 高性能

适用情况：

- 零售、通讯、银行、生物数据挖掘等等等

## What Kinds of Data can be Mined?

- 面向数据库的数据集合应用——关系数据库、数据仓库、事务型数据
- 高级数据集和高级应用——数据流、传感器数据、时间序列数据、多媒体数据、文本数据库、WWW等

## What Kinds of Patterns can be Mined?

Data Mining Functions:

### Generalization 一般化

- 信息综合与数据仓库组建——数据清理、数据变换、数据聚集、多维度数据模型
- 数据立方体技术
  - 数据立方体技术具有可扩展性(Scalable: Can be LARGER)的计算多维度聚合的方法：??实例化(Materializing)
  - OLAP
- 多维度的数据概念描述(教材P10)——数据特征化(隐含了数据聚合)与数据区分

### Association and Correlation Analysis 关联与相关分析

- 频率模式(Frequent patterns occurs frequency in itemset)
- 关联(Association)、相关(Correlation)、因果(Causality)

**Association refers to a more generalized term and correlation can be considered as a special case of association, where the relationship between the variables is linear in nature. Association is a relationship between two random variables which makes them statistically dependent. **

- 后续问题：如何在大量数据集中高效率地挖掘这样的模式与规则？如何使用这些模式进行分类、聚集和其他应用？

### Classification 分类

#### 分类与标签推测

- 基于训练样本建模
- 描述并区分各个类别和概念，以供之后推测用
- 预测某些未知的类标签

#### 关键方法

- 决策树：Decision Tree
- 朴素贝叶斯分类法：naive Bayesian classification
- 支持向量机：support vector machines
- 神经网络：neural netwoks
- 基于规则的分类：rule-based classfication
- 基于模式的分类：pattern-based classification
- 逻辑回归：logistic regression

### Cluster Analysis 聚类分析

- 无监督学习——无标签
- 规则：最大化本类内部相似度，最小化类间相似度

### Outlier Analysis 离群分析

- 离群(Outlier)：一个数据对象象不遵循这种数据普遍的行为
- 造成这种的现象的原因？噪声？例外？
- 方法：回归分析、聚类....??

### Time and Ordering: Sequential Pattern, Trend and Evolution Analysis 时间与顺序：顺序模式、趋势和发展分析

### Structure and Network Analysis 结构与网络分析

### Evaluation of Knowledge 知识评估(数据后处理)

---

## What Technologies are Used?

- 机器学习
- 模式识别
- 统计
- 可视化
- 高性能计算
- 数据库技术
- 算法
- 应用

## Major Issues in Data Mining

- 数据挖掘方法论(Mining Methodology)
- 用户交互
- 效率与可扩展性
- 数据类型多样化
- 数据挖掘与社会