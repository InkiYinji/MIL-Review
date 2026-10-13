[上一级](README.md)

# 序列与长程依赖

利用 Transformer、状态空间模型等建模长程实例依赖。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[GraphMamba](https://github.com/titizheng/GraphMamba)|[哈尔滨工业大学](https://scholar.google.com/citations?user=AJ5zl-wAAAAJ)|[PR](https://www.sciencedirect.com/science/article/pii/S0031320325004285)|GraphMamba: Whole slide image classification meets graph-driven selective state space model|以组内和跨组图 Mamba 建模不同层次的实例关系|WSI|
|[GMMamba](https://github.com/titizheng/GMMamba)|[哈尔滨工业大学](https://scholar.google.com/citations?user=AJ5zl-wAAAAJ)|[ICCV'25](https://openaccess.thecvf.com/content/ICCV2025/papers/Zheng_GMMamba_Group_Masking_Mamba_for_Whole_Slide_Image_Classification_ICCV_2025_paper.pdf)|GMMamba: Group masking Mamba for whole slide image classification|利用组内掩码Mamba进行选择性实例探索，并结合跨组超特征采样改善长程关系|WSI|
|[M3amba](https://github.com/titizheng/M3amba)|[哈尔滨工业大学](https://scholar.google.com/citations?user=AJ5zl-wAAAAJ)|[CVPR'25](https://openaccess.thecvf.com/content/CVPR2025/papers/Zheng_M3amba_Memory_Mamba_is_All_You_Need_for_Whole_Slide_CVPR_2025_paper.pdf)|M3amba: Memory Mamba is all you need for whole slide image classification|记忆驱动的Mamba网络，以充分探索实例之间的全局潜在关系|WSI|
|Pixel-Mamba|[浙江大学](https://scholar.google.com/citations?hl=zh-CN&user=uVV3rqcAAAAJ)|[ICCV'25](https://openaccess.thecvf.com/content/ICCV2025/papers/Qiu_Bridging_Local_Inductive_Bias_and_Long-Range_Dependencies_with_Pixel-Mamba_for_ICCV_2025_paper.pdf)|Bridging local inductive bias and long-range dependencies with pixel-Mamba for end-to-end whole slide image analysis|利用Mamba分层结合局部和全局信息，同时有效解决计算挑战|WSI|
|[**MambaMIL✳**](https://github.com/isyangshu/MambaMIL)|[香港科技大学](https://scholar.google.com/citations?user=6QlQF1oAAAAJ&hl=zh-CN&oi=sra)|[MICCAI'24](https://link.springer.com/chapter/10.1007/978-3-031-72083-3_28)|[MambaMIL: Enhancing long sequence modeling with sequence reordering in computational pathology](https://blog.csdn.net/weixin_44575152/article/details/143690996)|[在MIL中引入Mamba的长序列建模，并提出SR-Mamba和Bi-Mamba两个增强插件](https://blog.csdn.net/qq_32701507/article/details/136762360)|WSI|
|[MamMIL](https://github.com/Vison307/MamMIL)|[清华大学](https://scholar.google.com/citations?user=G_fXoMwAAAAJ)|[BIBM'24](https://ieeexplore.ieee.org/abstract/document/10822552/)|MamMIL: Multiple instance learning for whole slide images with state space models|以拓扑感知扫描将 WSI 图序列化，供 Mamba 建模|WSI|
|VINO|[复旦大学](https://scholar.google.com/citations?user=Xc6ehVAAAAAJ&hl=zh-CN&oi=sra)|AAAI'24|Transformer-based video-structure multi-instance learning for whole slide image classification|将WSI建模为病理学家的观察视频，并利用Transformer以分而治之的策略处理视频片段|WSI|
|[TransMIL](https://github.com/szc19990412/TransMIL)|[清华大学](https://scholar.google.com/citations?user=AGmtoloAAAAJ&hl=zh-CN&oi=sra)|NeurIPS‘21|[TransMIL: Transformer based correlated multiple instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/127608658)|基于Transformer的相关型MIL框架|WSI|
