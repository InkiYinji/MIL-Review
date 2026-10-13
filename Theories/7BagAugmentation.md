[上一级](README.md)

# 包构造与数据增强

通过伪包、包级采样和特征混合扩充或净化训练数据。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[DPBAug](https://github.com/JiuyangDong/DPBAug)|[哈尔滨工业大学](https://www.hit.edu.cn/)|[TMI'25](https://doi.org/10.1109/TMI.2025.3569941)|Disentangled pseudo-bag augmentation for whole slide image multiple instance learning|先按表型划分低噪声伪包，再跨切片融合增强训练|WSI|
|[MAP-MIL](https://github.com/Pikachu-one/MAP-MIL)|[东北林业大学](https://scholar.google.com/citations?hl=zh-CN&user=aHuB264AAAAJ)|[ESWA'25](https://www.sciencedirect.com/science/article/pii/S0957417425041405)|MAP-MIL: Dual-branch collaborative learning of mask enhancement and pseudo-bag generation for whole slide image classification|以掩码增强和注意力引导的伪包双分支协同训练|WSI|
|[PCR-MIL](https://github.com/JingjiaoLou/PCR-MIL)|山东大学|[MICCAI'25](https://papers.miccai.org/miccai-2025/paper/4174_paper.pdf)|PCR-MIL: Phenotype clustering reinforced multiple instance learning for whole slide image classification|按表型聚类构造低噪声伪包，并用强化学习优化特征提取|WSI|
|[PseMix](https://github.com/liupei101/PseMix)|电子科技大学|TMI‘24|Pseudo-bag mixup augmentation for multiple instance learning-based whole slide image classification|在伪包之间做 Mixup，扩充 WSI 弱监督训练样本|WSI|
|RankMix|[台湾省中央研究院](https://scholar.google.com/citations?user=7JwqUpYAAAAJ&hl=zh-CN&oi=sra)|[CVPR'23](https://openaccess.thecvf.com/content/CVPR2023/papers/Chen_RankMix_Data_Augmentation_for_Weakly_Supervised_Learning_of_Classifying_Whole_CVPR_2023_paper.pdf)|RankMix: Data augmentation for weakly supervised learning of classifying whole slide images with diverse sizes and imbalanced categories|在一对WSI中混合排序特征，以进行数据增强|WSI|
|[DTFD-MIL](https://github.com/hrzhang1123/DTFD-MIL)|[利物浦大学](https://scholar.google.com/citations?user=3bd8UIsAAAAJ&hl=zh-CN&oi=sra)|[CVPR'22](https://openaccess.thecvf.com/content/CVPR2022/html/Zhang_DTFD-MIL_Double-Tier_Feature_Distillation_Multiple_Instance_Learning_for_Histopathology_Whole_CVPR_2022_paper.html)|[DTFD-MIL: Double-tier feature distillation multiple instance learning for histopathology whole slide image classification](https://blog.csdn.net/weixin_44575152/article/details/124280361)|划分伪包并进行双层特征蒸馏，缓解训练包不足|WSI|
|[ReMix](https://github.com/TencentAILabHealthcare/ReMix)|[腾讯AI研究室/加州大学](https://scholar.google.com/citations?user=OYrpIa8AAAAJ&hl=zh-CN&oi=sra)|[MICCAI'22](https://arxiv.org/pdf/2207.01805)|ReMix: A general and efficient framework for multiple instance learning based whole slide image classification|先用原型压缩实例，再做潜空间特征混合增强|WSI|
