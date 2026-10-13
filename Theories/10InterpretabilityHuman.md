[上一级](README.md)

# 可解释性与人机协作

区分**解释模型**与**让专家改变模型**：热图、概念解释和临床工作流并不自动等于医生参与训练；只有能引入人工反馈或干预决策机制的方法才称为人机协作。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|iPathWS|[山西大学](https://www.sxu.edu.cn/)|[TPAMI'26](https://doi.org/10.1109/TPAMI.2026.3702808)|iPathWS: An integrated scalable system for explainable pathology diagnosis with spectral heterogeneity engine networks|把异质性建模、切片扫描和解释热图联成诊断系统；不属于医生反馈训练|WSI|
|[xMIL](https://github.com/bifold-pathomics/xMIL)|[柏林工业大学](https://www.tu.berlin/)|[MIA'26](https://doi.org/10.1016/j.media.2026.104148)|Beyond attention heatmaps: How to get better explanations for multiple instance learning models in histopathology|评估并改进 MIL 解释的忠实性；属于解释研究，不是专家反馈|WSI|
|[ProtoMIL](https://github.com/ss-sun/ProtoMIL)|[图宾根大学](https://uni-tuebingen.de/)|[MICCAI'25](https://doi.org/10.1007/978-3-032-05185-1_49)|Prototype-based multiple instance learning for gigapixel whole slide image classification|用稀疏概念解释预测，并允许专家修改概念以干预模型|WSI|
