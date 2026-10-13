[上一级](README.md)

# 多示例多标签（MIML）

输入是实例包，输出是**可同时成立的多个标签**。难点既包括包级多标签预测，也包括未知的“哪个实例支持哪个标签”关系。与 [MIPL](MIPL.md) 不同，这里的多个标签不只是候选项。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|D-MimlSvm|[南京大学 LAMDA](https://www.lamda.nju.edu.cn/)|[Artificial Intelligence'12](https://doi.org/10.1016/j.artint.2011.10.002)|Multi-instance multi-label learning|在正则化框架下直接建模实例包与多标签的关系，减少问题退化的信息损失|理论|
|MIMLBoost / MIMLSVM|[南京大学 LAMDA](https://www.lamda.nju.edu.cn/)|[NeurIPS'06](https://proceedings.neurips.cc/paper/2006/hash/8e489b4966fe8f703b5be647f1cbae63-Abstract.html)|Multi-instance multi-label learning with application to scene classification|形式化 MIML，并通过任务转化学习图像包的多个场景标签|场景分类|

2012 年期刊论文扩展了早期框架，并提出直接建模的 D-MimlSvm；上表将两篇按不同核心贡献呈现。
