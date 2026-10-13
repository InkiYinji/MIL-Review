[上一级](README.md)

# 表征与原型学习

改进实例或包表征，包括对比学习、自监督预训练、原型与概念学习。

Giga-SSL、HiDisc 属于支持 MIL 的病理图像表征预训练工作，并非包级聚合器。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|COMIL|[哈尔滨工业大学](https://titizheng.github.io/)|[KBS'25](https://www.sciencedirect.com/science/article/pii/S0950705125019744)|Collaborative optimization for whole slide image classification|以邻域对比学习优化实例表征，再由 Transformer 聚合|WSI|
|DPMIL|[华东理工大学](https://scholar.google.com/citations?user=XMIU7ygAAAAJ)|[ACM MM'25](https://dl.acm.org/doi/abs/10.1145/3746027.3755663)|[Dual-prototype learning in multiple instance learning for histopathology image classification](https://inkiyinji.blog.csdn.net/article/details/154157176)|同时建模全局共性与边界判别特征|WSI|
|[PacMIL](https://github.com/Baron-Huang/PacMIL)|新疆大学|[MIA'25](https://www.sciencedirect.com/science/article/pii/S1361841525004268)|A multi-instance learning network with prototype-instance adversarial contrastive for cervix pathology grading|端到端原型实例对抗对比学习|WSI|
|[ProtoMIL](https://github.com/ss-sun/ProtoMIL/tree/main)|[图宾根大学](https://scholar.google.com/citations?user=cyGvnh8AAAAJ)|[MICCAI'25](https://link.springer.com/chapter/10.1007/978-3-032-05185-1_49)|[Prototype-based multiple instance learning for gigapixel whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/153208675)|用稀疏自编码器发现可解释概念，以概念表征分类并支持人工干预|WSI|
|[**DGR-MIL✳**](https://github.com/ChongQingNoSubway/DGR-MIL)|[亚利桑那州立大学](https://scholar.google.com/citations?user=Se8aIO4YIp8C&hl=zh-CN&oi=sra)|[ECCV'24](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/05548.pdf)|[DGR-MIL: Exploring diverse global representation in multi-instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/143431511)|以多个全局向量汇总实例，保留包内表征多样性|WSI|
|[Giga-SSL★](https://github.com/trislaz/gigassl)|[巴黎科学与文学大学](https://scholar.google.com/citations?user=OAKoksYAAAAJ&hl=zh-CN&oi=sra)|CVPR’23|[Giga-SSL: Self-supervised learning for gigapixel images](https://blog.csdn.net/weixin_44575152/article/details/141940131)|从超大图像采样并增强实例集合，进行自监督对比预训练|WSI|
|[HiDisc](https://github.com/MLNeurosurg/hidisc)|[密歇根大学](https://scholar.google.com/citations?user=T9GuTDIAAAAJ&hl=zh-CN&oi=sra)|CVPR'23|[Hierarchical discriminative learning improves visual representations of biomedical microscopy](https://blog.csdn.net/weixin_44575152/article/details/141954874)|利用患者-WSI-区块这一层级结构信息来设置自监督学习中的对比损失|WSI|
|[ItS2CLR](https://github.com/Kangningthu/ItS2CLR)|[纽约大学](https://scholar.google.com/citations?user=F3F2qAkAAAAJ&hl=zh-CN&oi=sra)|CVPR'23|[Multiple instance learning via iterative self-paced supervised contrastive learning](https://inkiyinji.blog.csdn.net//article/details/133066363)|以自步筛选的实例伪标签开展监督对比学习，改善实例表征|WSI|
|[SMILES★](https://github.com/fulowl/smiles)|[东北大学](https://scholar.google.com/citations?user=LVRwELgAAAAJ&hl=zh-CN&oi=sra)|AAAI'23|[Robust self-supervised multi-instance learning with structure awareness](https://blog.csdn.net/weixin_44575152/article/details/131551473)|引入无监督对比学习来获取包表示|理论|
|[MuRCL](https://github.com/wwu98934/MuRCL)|厦门大学|TMI'22|[MuRCL: Multi-instance reinforcement contrastive learning for whole slide image classification](https://blog.csdn.net/weixin_44575152/article/details/128288963)|以对比学习训练实例表征，并用强化学习代理加速优化|WSI|
