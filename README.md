---

# 1 基本说明
本项目在于能够让大家能够更加快速地了解MIL这个领域，因此将从以下几个方面重点介绍MIL (这里不详细介绍每一篇文章，只做概述):
1. [MIL理论概述](Theories/README.md)
   - [传统MIL方法](Theories/Traditional.md) 
   - [注意力网络](Theories/Attention.md)
   - [自监督学习](Theories/SelfSupervised.md)
   - [因果推断/介入学习](Theories/CausalInference.md)
   - [强化学习](Theories/ReinforcementLearning.md)
   - [数据增强](Theories/DataEnhancement.md)
   - [对抗生成网络](Theories/GAN.md)
   - [大语言模型](Theories/LLM.md)
2. [MIL交叉领域](Extensions/README.md):
   - [多模态多示例 (M3IL)](Extensions/M3IL.md)
   - [多示例偏标签 (MIPL)](Extensions/MIPL.md)
   - [多示例多标签 (MIML)](Extensions/MIML.md)
   - [多示例对抗攻击及防御](Extensions/MILAttackDenfense.md)
   - [多示例正和无标签学习 (PU-MIL)](Extensions/PU-MIL.md)
   - [多示例分布外检测 (MIL-OOD)](Extensions/MIL-OOD.md)
   - [多示例主动学习](Extensions/MILActive.md)
3. [MIL应用领域](Applications/README.md):
   - [全幻灯片分类 (WSI)](Applications/WSI.md)
   - [视频异常检测 (VAD)](Applications/VAD.md)
   - [免疫库分类](Applications/IRC.md)

[**会议合集: https://github.com/Lionelsy/Conference-Accepted-Paper-List**](https://github.com/Lionelsy/Conference-Accepted-Paper-List)

[**代码合集: https://github.com/lingxitong/MIL_BASELINE**](https://github.com/lingxitong/MIL_BASELINE/tree/main)

[**Google学术: https://scholar.google.com/citations?user=JxgsypwAAAAJ&hl=zh-CN**](https://scholar.google.com/citations?user=JxgsypwAAAAJ&hl=zh-CN)

---
# 2 多示例背景介绍
**概述**: 多示例学习 (MIL) 是一种典型的弱监督学习，其输入的单个样本被称为**包** (bag)，包中包含多个实例 (instance)。在训练阶段，通常只有包的标签可知，而实例的标签不可知或者获取成本极高。因此，概括性的，MIL与传统机器学习的主要区别在于:
1. **弱监督场景**: 实例的数量巨大却没有标签，仅通过包标签来预测未知类，甚至预测实例标签是极具挑战性的;
2. **数据结构**: 包是多个实例的集合，实例可以是向量、图像、视频等任意结构，因此传统机器学习可以看作是MIL的一种特殊情况;

纵观MIL发展历程，其可以分为几个阶段:
1. 早期: 从Dietterich团队的药物活性预测研究开始，尝试直接使用传统的机器学习方法解决MIL问题;
2. 发展: 尝试MIL问题的转换，通常使用嵌入函数或包相似性度量来将其简化为传统的机器学习问题;
3. 深度: 利用深度学习的强大特征提取及表征能力，直接预测包的标签，这也是目前MIL研究的重点;
4. 应用: 考虑更多背景信息，如视频的时序、医疗图像相邻区块的关联性，以更好地处理实际任务;

---
# 3 注解
- **注1**: <font color=red>欢迎大家进一步交流，可以加入我建立的QQ群: 649325831</font>;
<div align=center>
  <img src="MIL-QQ.jpg" width="50%">
</div>

- **注2**: <font color=red>如果给出的文章包含代码，则可以点击其名称缩写获取</font>;
- **注3**: 承2，如果包含博客讲解，可以点击其全称获取;
- **注4**: 承3，如果包含论文原文，可以点击会议缩写名获取;
- **注5**: 一些缩写:
  - WSI: 全幻灯片分类 (医学领域，目前最热门的MIL应用);
  - VAD: 视频异常检测;
  - ECG: 心电图;
  - IRC: 免疫库分类;
- **注6**: 对于每一个小节，其侧重点有所不同:
    - 章节2 (理论MIL概述): 关注算法的实现细节;
    - 章节3 (MIL交叉领域): MIL与多标签、偏标签、对抗攻击、分布外检测的一些结合;
    - 章节4 (MIL应用概述): 着重数据集的说明及其相关处理;
- **注7**: 欢迎大家引用俺哩论文:
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