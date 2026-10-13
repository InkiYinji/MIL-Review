[上一级](README.md)

# 显微成像与高内涵筛选

显微镜图像和细胞高内涵成像（HCI）可构成非 WSI 的 MIL：实验孔/样本是包，视野或单细胞是实例。不同实验批次、孔和处理条件需要分层划分，不能把同一孔的细胞随机分进训练与测试。

|数据集|官方入口|适用点|
|:---|:---|:---|
|BBBC021|[Broad Bioimage Benchmark Collection](https://bbbc.broadinstitute.org/BBBC021)|MCF7 细胞药物处理的显微表型数据，可探索药物/剂量级聚合。|
|BBBC047|[Broad Bioimage Benchmark Collection](https://bbbc.broadinstitute.org/BBBC047)|大规模 Cell Painting 药物处理数据；需要明确图像、孔与处理标签的层级。|

这些是可用于构造 MIL 问题的原始资源；并不声称每个原始数据集都提供标准 MIL 划分。

[MicroMIL](../Theories/3RelationStructure.md) 针对常规光学显微镜视野构图，属于关系结构方法；不能把它的实验数据自动等同于上述 BBBC 数据集。

[MoMIL](../Theories/13TaskAwareObjectives.md) 则针对高内涵筛选中多个 assay 的稀疏标签；论文使用其专有 HCI 数据，不能把 BBBC021/047 写成它的原始实验数据。
