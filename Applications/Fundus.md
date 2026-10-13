[上一级](README.md)

# 眼底影像（Fundus）

眼底图像不是 WSI。MIL 可把局部视野或病灶候选区域作为实例，也可把双眼或多次拍摄组织为包；具体包定义由方法决定。

|数据集|官方入口|适用点与注意事项|
|:---|:---|:---|
|EyePACS / Diabetic Retinopathy Detection|[EyePACS](https://www.eyepacs.com/data-analysis)、[Kaggle 比赛](https://www.kaggle.com/competitions/diabetic-retinopathy-detection/data)|常用于糖尿病视网膜病变分级；比赛标签、图像质量和数据使用规则需按原版核对。|
|Messidor-2|[ADCIS](https://www.adcis.net/en/third-party/messidor2/)|常用于糖网病变评估；**官方图像发布不自带统一的 DR 分级标签**，论文采用的第三方标签须单独注明。|
|IDRiD|[Grand Challenge 官方页](https://idrid.grand-challenge.org/Home/)|糖网病变分级及病灶分割；原始精细标注是否进入训练，会改变弱监督设定。|

若研究以视觉语言提示或大模型引导为主，方法放在 [Multimodal](../Multimodal/README.md)，此处只提供数据入口和应用说明。

方法例子：[MSTNet](../Theories/3RelationStructure.md) 是单模态眼底图像方法；[GVL-MIL](../Multimodal/README.md) 则利用视觉语言模型进行新生儿眼底筛查。两者按机制进入不同主线，而不是因为“眼底”另起方法类。
