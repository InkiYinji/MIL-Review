[上一级](README.md)

# 免疫库分类（IRC）

免疫库可视为包，TCR/BCR 序列或克隆为实例；一个受检者的库规模巨大，序列丰度、批次与患者划分都影响结果。这里是 MIL 的生物序列应用，不与病理 WSI 混为一类。

## 常用数据入口

|数据集/资源|原始入口|适用点与注意事项|
|:---|:---|:---|
|Emerson CMV TCR repertoires|[immuneACCESS 原始研究数据](https://clients.adaptivebiotech.com/pub/Emerson-2017-NatGen)|CMV 血清状态与 TCR 库级分类；按受检者划分并核对去重、测序深度与标签。|
|DeepRC benchmark suites|[作者代码与数据说明](https://github.com/ml-jku/DeepRC)|包含真实 CMV、植入信号、模拟免疫测序等不同任务；不要把合成包当作真实患者数据。|

如使用多模态临床信息或标签消歧，方法见 [Multimodal](../Multimodal/README.md)；本页记录数据协议。
