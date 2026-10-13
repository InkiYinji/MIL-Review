[上一级](README.md)

# 实例选择与实例级学习

从包级标签中发现关键实例，或利用伪标签及少量实例标注学习。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[OODML](https://github.com/titizheng/OODML)|[哈尔滨工业大学](https://vilab.hit.edu.cn/)|[AAAI'25](https://ojs.aaai.org/index.php/AAAI/article/view/33154/35309)|[OODML: Whole slide image classification meets online pseudo-supervision and dynamic mutual learning](https://inkiyinji.blog.csdn.net/article/details/147376912)|在线更新实例伪标签与记忆表征，并通过动态互学习改进预测|WSI|
|PAMIL（伪标签注意力）|云南大学|[EAAI'25](https://www.sciencedirect.com/science/article/pii/S0952197624020670)|Pseudo-label attention-based multiple instance learning for whole slide image classification|用高低置信实例生成伪标签，引导注意力聚合与特征微调|WSI|
|[SMMILe](https://github.com/ZeyuGaoAi/SMMILe)|[剑桥大学](https://scholar.google.com/citations?user=CeP6dkcAAAAJ)|[Nature Cancer'25](https://www.nature.com/articles/s43018-025-01060-8.pdf)|SMMILe enables accurate spatial quantification in digital pathology using multiple-instance learning|基于超块进行实例级空间量化，同时完成切片级分类|WSI|
|PAMIL（动态策略）|[哈尔滨工业大学](https://vilab.hit.edu.cn/team.html)|CVPR'24|Dynamic policy-driven adaptive multi-instance learning for whole slide image classification|用奖励反馈动态选择实例，并联合优化特征表征与包级决策|WSI|
|LNPL-MIL|[清华大学](https://scholar.google.com/citations?user=AGmtoloAAAAJ&hl=zh-CN&oi=sra)|ICCV'23|LNPL-MIL: Learning from noisy pseudo labels for promoting multiple instance learning in whole slide image|筛选较可靠的实例伪标签，并用顺序感知 Transformer 聚合|WSI|
|[MHIM-MIL](https://github.com/DearCaat/MHIM-MIL/)|香港科技大学|[ICCV'23](https://openaccess.thecvf.com/content/ICCV2023/html/Tang_Multiple_Instance_Learning_Framework_with_Masked_Hard_Instance_Mining_for_ICCV_2023_paper.html)|[Multiple instance learning framework with masked hard instance mining](https://inkiyinji.blog.csdn.net/article/details/134808878)|用教师—学生网络和实例遮蔽挖掘难实例|WSI|
