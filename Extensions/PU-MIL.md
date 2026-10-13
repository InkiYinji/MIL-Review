[上一级](README.md)

# 正包与无标签学习（PU-MIL）

训练时只知道一部分**正包**，其余包没有标签；不能把无标签包直接视为负包。它与传统 MIL 的实例标签缺失叠加，形成包级标签也不完整的学习问题。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[**PU-MIL-AD✳**](https://github.com/Lorenzo-Perini/PU-MIL-AD)|[鲁汶大学](https://www.kuleuven.be/)|[KDD'23](https://doi.org/10.1145/3580305.3599409)|Learning from positive and unlabeled multi-instance bags in anomaly detection|调整自编码器目标，从正包与无标签包学习异常检测|异常检测|
