[上一级](README.md)

# 因果与稳健学习

针对混杂因素、分布变化或预测不确定性提升模型可靠性。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[FC-MIL](https://github.com/7FFDW/FCMIL)|[福建农林大学](https://www.fafu.edu.cn/)|[TMI'26](https://doi.org/10.1109/TMI.2026.3697015)|Frequency-aware causal regularization for multiple instance learning in whole slide image classification|在频域构造因果正则，削弱与标签偶然相关的切片纹理|WSI|
|[MFC-MIL](https://github.com/WissingChen/MFC-MIL)|[东北大学](https://www.neu.edu.cn/)|[ICLR'25](https://proceedings.iclr.cc/paper_files/paper/2025/file/22a94399f08a058383e9ef7516ed103f-Paper-Conference.pdf)|A multiscale frequency domain causal framework for enhanced pathological analysis|以多尺度频域记忆估计背景分布并实施因果介入|WSI|
|**CaMIL✳**|[华东师范大学](https://scholar.google.com/citations?user=whZnq5wAAAAJ&hl=zh-CN&oi=sra)|[AAAI'24](https://ojs.aaai.org/index.php/AAAI/article/view/27873)|[CaMIL: Causal multiple instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/137237682)|以前门调整构造介入预测，削弱病理图像中的伪相关|WSI|
|[CIMIL](https://github.com/centurion-crawler/CIMIL)|[厦门大学](https://scholar.google.com/citations?user=llXf3wUAAAAJ&hl=zh-CN&oi=sra)|AAAI'24|Boosting multiple instance learning models for whole slide image classification: A modelagnostic framework based on counterfactual inference|用反事实子包评估与分层搜索找到可靠实例及伪标签|WSI|
|[IBMIL](https://github.com/HHHedo/IBMIL)|[上海交通大学](https://scholar.google.com/citations?user=-ok791gAAAAJ&hl=zh-CN&oi=sra)|[CVPR'23](https://openaccess.thecvf.com/content/CVPR2023/html/Lin_Interventional_Bag_Multi-Instance_Learning_on_Whole-Slide_Pathological_Images_CVPR_2023_paper.html)|Interventional bag multi-instance learning on whole-slide pathological images|以后门调整进行包级介入训练，抑制上下文先验造成的伪相关|WSI|
|[CausalMIL](https://github.com/WeijiaZhang24/CausalMIL)|[东南大学](https://scholar.google.com/citations?hl=zh-CN&user=7jmAPvAAAAAJ&view_op=list_works&sortby=pubdate)|NeurIPS'22|[Multi-instance causal representation learning for instance label prediction and out-of-distribution generalization](https://inkiyinji.blog.csdn.net/article/details/131370219)|获得实例级因果表示并考虑OOD问题|理论|
