[上一级](README.md)

# 表征与原型学习

改进实例或包表征，包括对比学习、自监督预训练、原型与概念学习。

Giga-SSL、HiDisc 属于支持 MIL 的病理图像表征预训练工作，并非包级聚合器。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[MAMMOTH](https://github.com/mahmoodlab/mammoth)|[麻省理工学院](https://www.mit.edu/)|[ICLR'26](https://openreview.net/pdf?id=S5Io33pc78)|Mixture of mini experts: Overcoming the linear layer bottleneck in multiple instance learning|以轻量专家混合层替换通用特征到任务特征的线性瓶颈|WSI|
|[MR-Block](https://github.com/BearCleverProud/MR-Block)|[香港中文大学](https://www.cuhk.edu.hk/)|[ICLR'26](https://openreview.net/pdf/c5170a6d4ea855344df3dcb7083f48e3f5015ff5.pdf)|Exploiting low-dimensional manifold of features for few-shot whole slide image classification|沿病理预训练特征的低维流形适配少样本分类|WSI|
|[PTCMIL](https://github.com/ubc-tea/PTCMIL)|[不列颠哥伦比亚大学](https://www.ubc.ca/)|[MIA'26](https://doi.org/10.1016/j.media.2026.104013)|PTCMIL: Multiple instance learning via prompt token clustering for whole slide image analysis|用可学习提示 token 聚类实例表征；此处的 prompt 不是文本输入|WSI|
|[PacMIL](https://github.com/Baron-Huang/PacMIL)|[新疆大学](https://www.xju.edu.cn/)|[MIA'26](https://doi.org/10.1016/j.media.2025.103880)|A multi-instance learning network with prototype-instance adversarial contrastive for cervix pathology grading|以原型—实例对抗对比学习区分宫颈病理分级特征|WSI|
|DRE-SLCL|[中南大学](https://www.csu.edu.cn/)|[ACM MM'25](https://doi.org/10.1145/3746027.3755469)|Dynamic residual encoding with slide-level contrastive learning for end-to-end whole slide image representation|以动态残差编码和切片级对比学习优化端到端表征|WSI|
|Flow-MIL|[复旦大学](https://www.fudan.edu.cn/)|[ICCV'25](https://openaccess.thecvf.com/content/ICCV2025/html/Ma_Flow-MIL_Constructing_Highly-expressive_Latent_Feature_Space_For_Whole_Slide_Image_ICCV_2025_paper.html)|Flow-MIL: Constructing highly-expressive latent feature space for whole slide image classification using normalizing flow|以归一化流构建潜在语义空间，并用类特异原型增强聚合|WSI|
|COMIL|[哈尔滨工业大学](https://titizheng.github.io/)|[KBS'25](https://www.sciencedirect.com/science/article/pii/S0950705125019744)|Collaborative optimization for whole slide image classification|以邻域对比学习优化实例表征，再由 Transformer 聚合|WSI|
|DPMIL|[华东理工大学](https://scholar.google.com/citations?user=XMIU7ygAAAAJ)|[ACM MM'25](https://dl.acm.org/doi/abs/10.1145/3746027.3755663)|[Dual-prototype learning in multiple instance learning for histopathology image classification](https://inkiyinji.blog.csdn.net/article/details/154157176)|同时建模全局共性与边界判别特征|WSI|
|[**DGR-MIL✳**](https://github.com/ChongQingNoSubway/DGR-MIL)|[亚利桑那州立大学](https://scholar.google.com/citations?user=Se8aIO4YIp8C&hl=zh-CN&oi=sra)|[ECCV'24](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/05548.pdf)|[DGR-MIL: Exploring diverse global representation in multi-instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/143431511)|以多个全局向量汇总实例，保留包内表征多样性|WSI|
|[Giga-SSL★](https://github.com/trislaz/gigassl)|[巴黎科学与文学大学](https://scholar.google.com/citations?user=OAKoksYAAAAJ&hl=zh-CN&oi=sra)|CVPR’23|[Giga-SSL: Self-supervised learning for gigapixel images](https://blog.csdn.net/weixin_44575152/article/details/141940131)|从超大图像采样并增强实例集合，进行自监督对比预训练|WSI|
|[HiDisc](https://github.com/MLNeurosurg/hidisc)|[密歇根大学](https://scholar.google.com/citations?user=T9GuTDIAAAAJ&hl=zh-CN&oi=sra)|CVPR'23|[Hierarchical discriminative learning improves visual representations of biomedical microscopy](https://blog.csdn.net/weixin_44575152/article/details/141954874)|利用患者-WSI-区块这一层级结构信息来设置自监督学习中的对比损失|WSI|
|[ItS2CLR](https://github.com/Kangningthu/ItS2CLR)|[纽约大学](https://scholar.google.com/citations?user=F3F2qAkAAAAJ&hl=zh-CN&oi=sra)|CVPR'23|[Multiple instance learning via iterative self-paced supervised contrastive learning](https://inkiyinji.blog.csdn.net//article/details/133066363)|以自步筛选的实例伪标签开展监督对比学习，改善实例表征|WSI|
|[SMILES★](https://github.com/fulowl/smiles)|[东北大学](https://scholar.google.com/citations?user=LVRwELgAAAAJ&hl=zh-CN&oi=sra)|AAAI'23|[Robust self-supervised multi-instance learning with structure awareness](https://blog.csdn.net/weixin_44575152/article/details/131551473)|引入无监督对比学习来获取包表示|理论|
|[MuRCL](https://github.com/wwu98934/MuRCL)|厦门大学|TMI'22|[MuRCL: Multi-instance reinforcement contrastive learning for whole slide image classification](https://blog.csdn.net/weixin_44575152/article/details/128288963)|以对比学习训练实例表征，并用强化学习代理加速优化|WSI|
