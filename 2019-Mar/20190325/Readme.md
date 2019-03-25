# RQ及一些要点总结

## RQ

- LOC
- git diff
- 对git commit -m"" 中的commit信息，提取关键词，或情感分析，NLP语义分析，它是fixbug还是addfunc —— commit comment分类
- 定位release版本发布时间，分析版本间代码的区别(AST分析，贡献人员活跃度变化)
- 开发质量与ddl之间的关系

---

## Some Tips

### 什么是项目演化

- 主要是release版本间的增改删(可能存在没有release的大项目：kernel image) 衡量项目演化：基于一系列版本之间的diff的指标，由这些指标刻画

---

衡量标准，有时可以通过人工标记(审查)，调查问卷等社会工程学方式进行。

---

要把DM和ML中学习的一些方法应用到项目当中来。