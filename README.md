# 1 基本说明
本项目希望帮助读者快速建立 MIL 的方法地图，并找到相应论文、应用与数据入口。这里提供导航和简明机制概述，不逐篇复述论文。

**先看总览**：MIL 以一个包（bag）及其弱标签学习，包内实例（instance）通常缺少可靠标签。方法研究回答的是四个连续问题：如何构造包，如何学习并挑选实例证据，如何聚合实例之间的关系，以及如何让包级预测更稳健、可解释且高效。[单模态路线](Theories/README.md)按这些主要机制组织论文，传统 MIL 与注意力 MIL 固定为 1、2 类；跨模态信息或大模型实质参与学习的工作另进 [Multimodal](Multimodal/README.md)。WSI、乳腺 X 线、眼底、超声、视频和免疫库是**应用与数据**，不是与注意力/图网络并列的方法类别。

建议先读单模态总览与 1、2 类建立基线，再按研究问题选机制分支；要选数据集或复现实验，则到 Applications 核对包定义、原始标签、患者级划分和数据授权。一个方法只在主贡献所属页面保留一行，特殊方向（如真实的人类反馈、概率校准）仍单独呈现。

1. [单模态 MIL 方法路线](Theories/README.md)：从[传统方法](Theories/1Traditional.md)和[注意力网络✳](Theories/2Attention.md)入门，按“包构造—实例表征与选择—关系聚合—可靠性与效率”追踪核心机制；**不限于 WSI**，其他单模态应用也按主要方法归类。
2. [Multimodal：大模型与多模态 MIL](Multimodal/README.md)：单列视觉语言模型、大模型引导及额外模态参与训练或推理的方法。
3. [MIL交叉领域](Extensions/README.md)
   - [多示例偏标签 (MIPL)](Extensions/MIPL.md)
   - [多示例多标签 (MIML)](Extensions/MIML.md)
   - [多示例对抗攻击及防御](Extensions/MILAttackDefense.md)
   - [多示例正和无标签学习 (PU-MIL)](Extensions/PU-MIL.md)
   - [多示例分布外检测 (MIL-OOD)](Extensions/MIL-OOD.md)
   - [多示例主动学习](Extensions/MILActive.md)
4. [MIL应用领域](Applications/README.md)
   - [病理全切片 (WSI)](Applications/WSI.md)
   - [乳腺 X 线影像](Applications/Mammography.md)
   - [眼底影像](Applications/Fundus.md)
   - [超声影像](Applications/Ultrasound.md)
   - [视频异常检测 (VAD)](Applications/VAD.md)
   - [免疫库分类](Applications/IRC.md)

[**会议合集：https://github.com/Lionelsy/Conference-Accepted-Paper-List**](https://github.com/Lionelsy/Conference-Accepted-Paper-List)

[**代码合集：https://github.com/lingxitong/MIL_BASELINE**](https://github.com/lingxitong/MIL_BASELINE/tree/main)

---
# 2 多示例背景介绍
**概述**：多示例学习 (MIL) 是一种典型的弱监督学习，其输入的单个样本被称为**包** (bag)，包中包含多个实例 (instance)。在训练阶段，通常只有包的标签可知，而实例的标签不可知或者获取成本极高。因此，概括性的，MIL与传统机器学习的主要区别在于：
1. **弱监督场景**：实例的数量巨大却没有标签，仅通过包标签来预测未知类，甚至预测实例标签是极具挑战性的；
2. **数据结构**：包是多个实例的集合，实例可以是向量、图像、视频等任意结构，因此传统机器学习可以看作是MIL的一种特殊情况；

纵观MIL发展历程，其可以分为几个阶段：
1. 早期：从Dietterich团队的药物活性预测研究开始，尝试直接使用传统的机器学习方法解决MIL问题；
2. 发展：尝试MIL问题的转换，通常使用嵌入函数或包相似性度量来将其简化为传统的机器学习问题；
3. 深度：利用深度学习的强大特征提取及表征能力，直接预测包的标签，这也是目前MIL研究的重点；
4. 应用：考虑更多背景信息，如视频的时序、医疗图像相邻区块的关联性，以更好地处理实际任务；

---
# 3 注解
- **注1：欢迎大家进一步交流，可以加入我建立的QQ群：649325831**；
<div align=center>
  <img src="MIL-QQ.jpg" width="50%">
</div>

- **注2：如果给出的文章包含代码，则可以点击其名称缩写获取**；
- **注3**：承2，如果包含博客讲解，可以点击其全称获取；
- **注4**：承3，如果包含论文原文，可以点击会议缩写名获取；
- **注5**：一些缩写：
  - WSI：病理全切片图像，可用于分类、分级、预后等多种 MIL 任务；
  - VAD：视频异常检测；
  - ECG：心电图；
  - IRC：免疫库分类；
- **注6**：四个入口的侧重点不同：
    - [单模态 MIL 方法路线](Theories/README.md)：不限于 WSI，梳理核心思路、技术关系与阅读顺序；
    - [大模型与多模态 MIL](Multimodal/README.md)：额外模态或预训练大模型如何参与 MIL；
    - [MIL 交叉领域](Extensions/README.md)：MIL 与多标签、偏标签、对抗攻击、分布外检测等任务的结合；
    - [MIL 应用领域](Applications/README.md)：应用场景、数据集及其处理；
- **注7**：**✳标识的方法适合入门，★标识的方法相对简单**；
- **注8**：欢迎大家引用俺哩论文：
```javascript
@article{Zhang:2024:data:115,
author		=	{Zhang, Yu-Xuan and Zhou, Zhengchun and He, Xingxing and Adhikary, Avik Ranjan and Dutta, Bapi},
title		=	{Data-driven knowledge fusion for deep multi-instance learning},
journal		=	{{IEEE} Transactions on Neural Networks and Learning Systems},
year		=	{2024},
pages		=	{1--15},
}
```
```javascript
@article{Zhang:2023:interpreting:109725,
author      =   {Zhang, Yu-Xuan and Meng, Hua and Cao, Xue-Mei and Zhou, Zhengchun and Yang, Mei and Adhikary, Avik Ranjan},
title       =   {Interpreting vulnerabilities of multi-instance learning to adversarial perturbations},
journal     =   {Pattern Recognition},
year        =   {2023},
pages       =   {109725},
volume      =   {142},
}
```
```javascript
@article{Yang:2021:multi:54565467,
author      =   {Yang, Mei and Zhang, Yu-Xuan and Wang, Xizhao and Min, Fan},
title       =   {Multi-instance ensemble learning with discriminative bags},
journal     =   {IEEE Transactions on Systems, Man, and Cybernetics: Systems},
pages       =   {5456--5467},
year        =   {2021},
volume      =   {52},
number      =   {9},
}
```
