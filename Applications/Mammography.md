[上一级](README.md)

# 乳腺 X 线影像（Mammography）

这是**乳腺影像应用**，不是“乳腺 MIL”独立方法类，也不要与乳腺病理 WSI 混淆。可把一项检查的多视图或从大图裁出的候选区域作为一个包；具体标签与包单位须以论文为准。

|数据集|官方入口|适用点与注意事项|
|:---|:---|:---|
|CBIS-DDSM|[TCIA](https://www.cancerimagingarchive.net/collection/cbis-ddsm/)|整理过的扫描胶片乳腺 X 线资料，包含病灶及病理信息；不是原生数字乳腺摄影。|
|VinDr-Mammo|[PhysioNet](https://physionet.org/content/vindr-mammo/1.0.0/)|数字乳腺摄影、多视图检查及 BI-RADS / 病灶标注；需注册并签署使用协议。|
|EMBED Open Data|[Emory 官方说明](https://docs.hitilab.com/docs/datasets/embed)|含影像、检查与临床元数据；公开部分只是全量 EMBED 的子集，需遵守研究用途协议。|

不要把“视图”“乳房”“患者”三个标签层级混用；多视图 MIL 尤其要按患者划分训练与测试。[病理乳腺数据](WSI.md)另见 WSI 页面。

方法例子：[FPN-MIL](../Theories/2Attention.md) 将多尺度局部证据用于高分辨率乳腺 X 线分类；方法收在注意力机制页，本页不重复其文献行。
