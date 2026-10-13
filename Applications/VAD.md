[上一级](README.md)

# 视频异常检测（VAD）

本页记录视频场景中的 MIL 应用；视频片段或时间窗可作为实例，整段视频作为包。使用视觉语言提示的 PE-MIL 见[大模型与多模态 MIL](../Multimodal/README.md)，此处不重复收录。

## 常见数据集

|数据集|原始入口|适用点与注意事项|
|:---|:---|:---|
|UCF-Crime|[UCF-CRCV 官方项目](https://www.crcv.ucf.edu/research/real-world-anomaly-detection-in-surveillance-videos/)|长时监控视频异常检测的常见弱监督基准；核对使用的是原始视频、片段特征还是二次整理版本。|
|XD-Violence|[作者数据集主页](https://roc-ng.github.io/XD-Violence/)|暴力事件检测，可包含音视频信息；纯视觉与音视频融合不能视作同一输入设定。|
|ShanghaiTech Campus|[发布实验室](https://svip-lab.github.io/dataset/campus_dataset.html)|校园监控异常检测资源；原始半监督协议与后续弱监督重划分不能直接比较。|

训练时只有视频级标签而测试时评估片段/帧定位，是常见但并非唯一的 VAD-MIL 协议。应注明异常类别、特征提取器、弱监督划分和是否使用音频/文本。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|CHEESE|[大连理工大学](https://scholar.google.com/citations?user=HDFA2VYAAAAJ&hl=zh-CN&oi=sra)|[TCDS'24](https://doi.org/10.1109/TCDS.2024.3349705)|Multiple instance learning for cheating detection and localization in online examinations|融合姿态、视线等特征，通过时空图定位视频中的异常行为|视频异常检测|
