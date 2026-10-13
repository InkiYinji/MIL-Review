[上一级](README.md)

# 注意力网络

以实例权重分配或注意力聚合为主要创新的方法。

ABMIL/GAMIL 是这一方向的入门起点。本页只收录注意力机制本身是主要贡献的方法；其他论文按其主要思路归类。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[TDA-MIL](https://github.com/agentdr1/TDA_MIL)|[雷根斯堡大学](https://scholar.google.com/citations?user=ErWW2sgAAAAJ)|[MICCAI'25](https://link.springer.com/chapter/10.1007/978-3-032-04927-8_62)|[Top-down attention-based multiple instance learning for whole slide image analysis](https://inkiyinji.blog.csdn.net/article/details/153883793)|先学习全局表示，再将任务相关实例回注注意力模块细化预测|WSI|
|[**ACMIL✳**](https://github.com/dazhangyu123/ACMIL)|[浙江大学](https://scholar.google.com/citations?user=xsENLrkAAAAJ&hl=zh-CN&oi=sra)|[ECCV'24](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/06954.pdf)|[Attention-challenging multiple instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/145161250)|以多分支注意力发现不同病灶，并随机遮蔽高权重实例|WSI|
|**AMD-MIL★**|[清华大学](https://scholar.google.com/citations?user=5lNlpagAAAAJ&hl=zh-CN&oi=sra)|ACM MM'24|[Agent aggregator with mask denoise mechanism for histopathology whole slide image analysis](https://blog.csdn.net/weixin_44575152/article/details/142062377)|代理注意力机制的改进及掩码去噪|WSI|
|[**CAMIL✳**](https://github.com/olgarithmics/ICLR_CAMIL)|[英国伦敦癌症研究所](https://scholar.google.com/citations?user=AkaRnp4AAAAJ&hl=zh-CN&oi=sra)|[ICLR'24](https://arxiv.org/pdf/2305.05314)|[CAMIL: Context-aware multiple instance learning for cancer detection and subtyping in whole slide images](https://blog.csdn.net/weixin_44575152/article/details/143385249)|以邻域约束注意力融入上下文信息，改善病灶识别|WSI|
|[**DSMIL★**](https://github.com/binli123/dsmil-wsi)|[威斯康星大学](https://scholar.google.com/citations?user=C9DtTm0AAAAJ&hl=zh-CN&oi=sra)|CVPR'21|[Dual-stream multiple instance learning network for whole slide image classification with self-supervised contrastive learning](https://inkiyinji.blog.csdn.net/article/details/125661028)|结合实例分类流与注意力聚合流，并用自监督对比学习预训练|WSI|
|[LAMIL](https://github.com/xsshi2015/Loss-Attention)|[佛罗里达大学](https://scholar.google.com/citations?user=-TQZLMcAAAAJ&hl=zh-CN&oi=sra)|AAAI'20|[Loss-based attention for deep multiple instance learning](https://inkiyinji.blog.csdn.net/article/details/119548407)|额外添加实例损失优化模型且提供理论证明|理论|
|[**ABMIL&GAMIL✳**](https://github.com/AMLab-Amsterdam/AttentionDeepMIL)|[阿姆斯特丹大学](https://scholar.google.com/citations?user=KNJIRGkAAAAJ&hl=zh-CN&oi=sra)|ICML'18|[Attention-based deep multiple instance learning](https://inkiyinji.blog.csdn.net/article/details/115341529)|设计了两种注意力机制来捕捉包中的关键实例|理论|
