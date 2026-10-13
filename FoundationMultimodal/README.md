[上一级](../README.md)

# 大模型与多模态 MIL

这里收录利用**额外模态、文本语义或预训练大模型**改变 MIL 学习过程的方法，与[单模态 MIL 方法路线](../Theories/README.md)并列。判断时同时记录训练和推理阶段：有的方法训练时借助另一模态，部署时仍只输入 WSI；有的方法在推理时融合图像与临床信息。

每篇论文在本页只出现一次。视觉语言模型同时属于“大模型”和“多模态”时，按其主要贡献选择下面的小节，不重复列表。

## 视觉语言与大模型引导

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[CoD-MIL](https://github.com/Jiangbo-Shi/CoD-MIL)|[西安交通大学](https://scholar.google.com/scholar?hl=zh-CN&as_sdt=0%2C5&q=CoD-MIL%3A+Chain-of-Diagnosis+Prompting+Multiple+Instance+Learning+for+Whole+Slide+Image+Classification&btnG=)|TMI'24|[CoD-MIL: Chain-of-diagnosis prompting multiple instance learning for whole slide image classification](https://blog.csdn.net/weixin_44575152/article/details/143690996)|用诊断链文本提示引导不同尺度的病理图像表征与聚合|WSI|
|[ViLa-MIL](https://github.com/Jiangbo-Shi/ViLa-MIL)|[西安交通大学](https://scholar.google.com/citations?user=FhR6erIAAAAJ)|[CVPR'24](https://openaccess.thecvf.com/content/CVPR2024/html/Shi_ViLa-MIL_Dual-scale_Vision-Language_Multiple_Instance_Learning_for_Whole_Slide_Image_CVPR_2024_paper.html)|ViLa-MIL: Dual-scale vision-language multiple instance learning for whole slide image classification|用大模型生成双尺度文本提示，结合视觉语言模型分析 WSI|WSI|
|[PE-MIL](https://github.com/Junxi-Chen/PE-MIL)|[中国科学院](https://scholar.google.com/citations?user=kVhdLkcAAAAJ)|CVPR'24|Prompt-enhanced multiple instance learning for weakly supervised video anomaly detection|以异常语义提示引导视频实例特征，进行弱监督异常检测|VAD|

## 多模态融合与预训练

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[PROGPATH](https://github.com/Valeyards/ProgPath)|[四川大学](https://scholar.google.com/citations?user=iJTVJf8AAAAJ)|[STTT'25](https://www.nature.com/articles/s41392-025-02374-w)|Pancancer outcome prediction via a unified weakly supervised deep learning model|融合 WSI 表征与临床变量，预测跨癌种预后|WSI + 临床|
|[LaDM3IL✳](https://github.com/Josie-xufan/LaDM3IL)|[上海科技大学](https://scholar.google.com/citations?user=7XOW0wcAAAAJ&hl=zh-CN)|AAAI'24|[A label disambiguation-based multimodal massive multiple instance learning](https://inkiyinji.blog.csdn.net/article/details/137521297)|通过标签消歧学习多模态免疫库包表示|IRC|
|[MDDP](https://github.com/lhaof/MDDP)|[香港中文大学](https://scholar.google.com/citations?user=ugBEYC4AAAAJ)|[ACM MM'24](https://doi.org/10.1145/3664647.3680882)|Multi-modal denoising diffusion pre-training for whole-slide image classification|以 H&E/IHC 配对预训练特征，推理时只需 H&E 图像|WSI|
|[AMIGO](https://github.com/raminnakhli/amigo)|[不列颠哥伦比亚大学](https://scholar.google.com/citations?user=8PZHgzUAAAAJ&hl=zh-CN&oi=sra)|[CVPR'23](https://openaccess.thecvf.com/content/CVPR2023/papers/Nakhli_Sparse_Multi-Modal_Graph_Transformer_With_Shared-Context_Processing_for_Representation_Learning_CVPR_2023_paper.pdf)|Sparse multi-modal graph transformer with shared-context processing for representation learning of giga-pixel images|融合不同标记染色图像的细胞图，学习患者级组织表征|多标记 IHC|
|MAMIL|武汉理工大学|KBS'23|Multimodal multi-instance learning for long-term ECG classification|融合多模态长时心电信号，进行包级分类|ECG|

“领域”用于标明应用或输入组合，不代替论文的主要分类；例如 MDDP 的多模态信息用于训练，实际推理仍是单张 H&E WSI。
