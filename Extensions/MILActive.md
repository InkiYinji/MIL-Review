[上一级](README.md)

# 主动学习与 MIL

在有限标注预算下，主动学习选择值得标注的包、图像或实例，以提高后续模型效益。这里关注**查询策略**；病理专家直接修正证据并参与迭代训练，则主要归入[可解释性与人机协作](../Theories/10InterpretabilityHuman.md)。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[MIDL](https://github.com/WanFang13/MIDL)|[中国科学院大学](https://www.ucas.ac.cn/)等|[TPAMI'23](https://doi.org/10.1109/TPAMI.2023.3277738)|Multiple instance differentiation learning for active object detection|将未标注图像视为实例包，联合实例与图像不确定性选择标注对象|目标检测|

> MIDL 借用包级建模服务于主动目标检测，并非只用包级弱标签训练的典型 MIL；保留于交叉方向，避免误归入单模态 MIL 核心机制表。
