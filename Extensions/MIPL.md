[上一级](README.md)

# 多示例偏标签（MIPL）

每个样本同时是**实例包**和**候选标签集**：包内关键实例未知，候选标签中也只有一个真实标签。核心是联合处理实例定位与标签消歧；不要与可有多个真实标签的 [MIML](MIML.md) 混淆。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[MIPLMA](https://palm.seu.edu.cn/zhangml/files/MIPLMA.zip)|[东南大学](https://palm.seu.edu.cn/zhangml/) / [纽卡斯尔大学](https://www.newcastle.edu.au/)|[NeurIPS'24](https://proceedings.neurips.cc/paper_files/paper/2024/hash/2e5a74735e5ada01d85afbb49caad36f-Abstract-Conference.html)|Multi-instance partial-label learning with margin adjustment|同时调整注意力分数与候选/非候选标签的预测间隔|理论|
|[PROMIPL](https://palm.seu.edu.cn/zhangml/files/ProMIPL.rar)|[东南大学](https://palm.seu.edu.cn/zhangml/)|[ICDM'24](https://palm.seu.edu.cn/zhangml/files/ICDM%2724.pdf)|PROMIPL: A probabilistic generative model for multi-instance partial-label learning|由概率生成过程推断包的潜在真实标签|理论|
|[ELIMIPL](https://palm.seu.edu.cn/zhangml/files/ELIMIPL.rar)|[东南大学](https://palm.seu.edu.cn/zhangml/) / [纽卡斯尔大学](https://www.newcastle.edu.au/)|[IJCAI'24](https://www.ijcai.org/proceedings/2024/0550)|Exploiting conjugate label information for multi-instance partial-label learning|利用候选与非候选标签的互补信息改进消歧|理论|
|[MIPLGP](https://palm.seu.edu.cn/zhangml/files/MIPLGP.rar)|[东南大学](https://palm.seu.edu.cn/zhangml/) / [纽卡斯尔大学](https://www.newcastle.edu.au/)|[SCIS'24](https://doi.org/10.1007/s11432-023-3771-6)|Multi-instance partial-label learning: Towards exploiting dual inexact supervision|提出 MIPL 设置，以高斯过程学习实例与候选标签的双重弱监督|理论|
|[**DEMIPL★**](https://github.com/tangw-seu/DEMIPL)|[东南大学](https://palm.seu.edu.cn/zhangml/) / [纽卡斯尔大学](https://www.newcastle.edu.au/)|[NeurIPS'23](https://proceedings.neurips.cc/paper_files/paper/2023/hash/b1917a4bcfab403c3cdd6c6bbaf9fda0-Abstract-Conference.html)|Disambiguated attention embedding for multi-instance partial-label learning|注意力嵌入包表示，并以动量策略识别真实标签|理论|
