[上一级](README.md)

# 效率、蒸馏与训练稳定性

主问题是如何减少高分辨率推理或大包训练成本，或通过蒸馏与训练策略提高可扩展性；使用注意力只是手段时不归入第 2 类。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|HAFD-MIL|[华东理工大学](https://www.ecust.edu.cn/)|[KBS'26](https://doi.org/10.1016/j.knosys.2026.116286)|Improving multi-instance learning with hierarchical attention and frequency-domain hard sample distillation|结合层级注意力与频域困难样本蒸馏，缓解注意力过度集中|WSI|
|CICS|[哈尔滨工业大学](https://www.hit.edu.cn/)|[AAAI'26](https://ojs.aaai.org/index.php/AAAI/article/view/38350)|Content-aware information compression and selection for whole slide image analysis|压缩冗余实例，再结合全局邻近信息选择有用证据|WSI|
|MIL-Merging|[巴黎电信学院](https://www.telecom-paris.fr/)|[MICCAI'25](https://papers.miccai.org/miccai-2025/0759-Paper4644.html)|Reducing variability of multiple instance learning methods for digital pathology|融合多次训练的 MIL 模型，降低随机初始化带来的性能波动|WSI|
|[HDMIL](https://github.com/JiuyangDong/HDMIL)|[哈尔滨工业大学](https://www.hit.edu.cn/)|[CVPR'25](https://openaccess.thecvf.com/content/CVPR2025/html/Dong_Fast_and_Accurate_Gigapixel_Pathological_Image_Classification_with_Hierarchical_Distillation_CVPR_2025_paper.html)|Fast and accurate gigapixel pathological image classification with hierarchical distillation multi-instance learning|由低分辨率筛查向高分辨率证据蒸馏，降低切片推理成本|WSI|
|DPGS-DMGC|[湖州学院](https://www.zjhzu.edu.cn/)|[ICML'25](https://proceedings.mlr.press/v267/wu25ae.html)|Distributed parallel gradient stacking (DPGS): Solving whole slide image stacking challenge in multi-instance learning|通过分布式梯度堆叠与压缩训练长度不一的大包|WSI|
|[ASMIL](https://github.com/Linfeng-Ye/ASMIL)|[多伦多大学](https://www.utoronto.ca/)|[ICLR'26](https://openreview.net/pdf?id=CYmjrbQRyM)|ASMIL: Attention-stabilized multiple instance learning for whole slide imaging|以锚模型稳定跨轮次注意力，抑制过度集中与过拟合|WSI|
|AGKD|[电子科技大学](https://www.uestc.edu.cn/)|[PR'26](https://doi.org/10.1016/j.patcog.2026.113642)|Attention-guided knowledge distillation based deep multiple instance learning for gigapixel whole slide image analysis|用注意力引导知识蒸馏，在切片级任务中传递关键实例信息|WSI|
