# 论文概述

## 摘要

通过向使用github的开发者使用一种数据挖掘算法：根据他们的行为数据，向他们推荐他们感兴趣的项目。这种数据挖掘的根据是，现如今大多数开发者都依赖于大量的开源开发框架来进行软件开发。本文尝试去探索这样的算法，以实现相关代码库的推荐功能。尝试回答这样三个问题：

- 1 什么样的用户行为数据适合用来做相关项目的推荐。
- 2 通过用户行为数据推荐的数据仓库之间有什么关联。
- 3 项目类型如何影响推荐的结果。

- 使用向量相似法，去评估项目间的关联性


## 研究设计

### 数据

  从github上选择了五种最常见的操作作为用户的行为数据

- 1 **fork**

- 2 **Watch**

- 3 **Issues Comment**  :在处理行为数据的过程中，将发起问题讨论和评论问题讨论都看作相同的行为对待。

- 4 **Pull-Request** 

- 5 **Member**：成为某个项目的核心成员  

### 方法

基本原理：通过比较两个相关项目中用户行为数据的相似程度来评估两个项目的相关度。可以将步骤概括如下：

- 1 用户向量：对于某个行为（比如fork), 如果某个用户k对某个仓库（项目）有fork行为，那么fork(k) = 1, 否则为0.

- 2 两个项目在某个行为上的相似分采用cos距离描述

- 3 对每一个项目，都针对它对其他项目进行分级（用相似分）

### 研究结果

#### 回答第一个问题：

通过对每个项目自己的相似分排名表计算平均分，可以得到五张表，表的走势恰好回答了问题，Fork、Watch, Pull-Request和Member是比较适合用来做推荐的。

#### 回答第二个问题

关联大致分为三种：依赖关系，协作关系和相似关系，那么向用户推荐的话也分为这三种类型推荐。其中：

- fork 和 watch 适合作为协作关系和相似项目的推荐。

- Member和Pull-Request适合作为依赖关系推荐。

#### 回答第三个问题

用户的行为数据在推荐项目时，对于库或者内核框架项目的推荐更准确，对于app开发项目的推荐不太有效。