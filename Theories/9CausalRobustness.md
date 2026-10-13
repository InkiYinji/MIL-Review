[上一级](README.md)

# 因果与稳健学习

针对混杂因素、分布变化或预测不确定性提升模型可靠性。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|[SIB-MIL](https://github.com/HKU-MedAI/SIB-MIL)|[香港大学](https://scholar.google.com/citations?user=YWyE2RcAAAAJ&hl=zh-CN&oi=sra)|[TMI'25](https://ieeexplore.ieee.org/abstract/document/11271037/)|SIB-MIL: Sparsity-induced bayesian neural network for robust multiple instance learning on whole slide image analysis|以稀疏贝叶斯建模表示不确定性，增强 WSI 分类稳健性|WSI|
|**CaMIL✳**|[华东师范大学](https://scholar.google.com/citations?user=whZnq5wAAAAJ&hl=zh-CN&oi=sra)|[AAAI'24](https://ojs.aaai.org/index.php/AAAI/article/view/27873)|[CaMIL: Causal multiple instance learning for whole slide image classification](https://inkiyinji.blog.csdn.net/article/details/137237682)|以前门调整构造介入预测，削弱病理图像中的伪相关|WSI|
|[CIMIL](https://github.com/centurion-crawler/CIMIL)|[厦门大学](https://scholar.google.com/citations?user=llXf3wUAAAAJ&hl=zh-CN&oi=sra)|AAAI'24|Boosting multiple instance learning models for whole slide image classification: A modelagnostic framework based on counterfactual inference|用反事实子包评估与分层搜索找到可靠实例及伪标签|WSI|
|[IBMIL](https://github.com/HHHedo/IBMIL)|[上海交通大学](https://scholar.google.com/citations?user=-ok791gAAAAJ&hl=zh-CN&oi=sra)|[CVPR'23](https://openaccess.thecvf.com/content/CVPR2023/html/Lin_Interventional_Bag_Multi-Instance_Learning_on_Whole-Slide_Pathological_Images_CVPR_2023_paper.html)|Interventional bag multi-instance learning on whole-slide pathological images|以后门调整进行包级介入训练，抑制上下文先验造成的伪相关|WSI|
|[CausalMIL](https://github.com/WeijiaZhang24/CausalMIL)|[东南大学](https://scholar.google.com/citations?hl=zh-CN&user=7jmAPvAAAAAJ&view_op=list_works&sortby=pubdate)|NeurIPS'22|[Multi-instance causal representation learning for instance label prediction and out-of-distribution generalization](https://inkiyinji.blog.csdn.net/article/details/131370219)|获得实例级因果表示并考虑OOD问题|理论|
