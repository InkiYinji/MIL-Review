[上一级](README.md)

# 任务结构与临床目标

当论文的主要创新来自**序数分期、特定分级规则或跨癌种预后目标**，而非通用聚合器时放在这里；应用数据集本身仍见应用领域页面。

|方法名|团队|期刊/会议|全称|思想|领域|
|:---|:---|:---|:---|:---|:---|
|STEPH|[湖南大学](https://www.hnu.edu.cn/)|[CVPR'26](https://openaccess.thecvf.com/content/CVPR2026/html/Liu_Sparse_Task_Vector_Mixup_with_Hypernetworks_for_Efficient_Knowledge_Transfer_CVPR_2026_paper.html)|Sparse task vector mixup with hypernetworks for efficient knowledge transfer in whole-slide image prognosis|稀疏融合跨癌种任务向量，将预后知识迁移到目标癌种|WSI|
|[MPEM](https://github.com/Shiku-Kaito/Learning-from-Majority-Label-A-Novel-Problem-in-Multi-class-Multiple-Instance-Learning)|[九州大学](https://www.kyushu-u.ac.jp/en/)|[PR'26](https://doi.org/10.1016/j.patcog.2025.112425)|Learning from majority label: A novel problem in multi-class multiple-instance learning|定义多数类决定包标签的 MIL 问题，并剔除少数类实例强化学习|通用 MIL|
|[AceMIL](https://github.com/LSJ-i/AceMIL)|[复旦大学](https://www.fudan.edu.cn/)|[CVPR Findings'26](https://openaccess.thecvf.com/content/CVPR2026F/html/Li_AceMIL_Ordinal-Aware_Multiple_Instance_Learning_for_Pathological_Progression_Analysis_CVPRF_2026_paper.html)|AceMIL: Ordinal-aware multiple instance learning for pathological progression analysis|以序数软标签和阶段聚合学习病理进展，避免把相邻分级视为无关类别|WSI|
|[DSPA-MIL](https://github.com/AlexNmSED/DSPA-MIL)|[大连理工大学](https://www.dlut.edu.cn/)|[MIA'26](https://doi.org/10.1016/j.media.2026.104005)|Dual selective Gleason pattern-aware multiple instance learning with uncertainty regularization for grade group prediction in histopathology images|围绕 Gleason 模式选择证据，并以不确定性正则预测分级组|WSI|
|GAMINN|[同济大学附属上海市肺科医院](https://www.shsfkyy.com/)|[npj Digital Medicine'25](https://doi.org/10.1038/s41746-025-01470-z)|Whole slide image based deep learning refines prognosis and therapeutic response evaluation in lung adenocarcinoma|用图注意力 MIL 预测肺腺癌复发风险，辅助治疗获益分层|WSI|
|MoMIL|[Janssen R&D](https://www.jnj.com/)|[MICCAI'25](https://papers.miccai.org/miccai-2025/0578-Paper1746.html)|MoMIL: Mixture of multi-instance learners for modeling multiple compound activities in high content imaging|共享高内涵图像表征并设置实验目标特异 MIL 分支，应对稀疏的多实验标签|高内涵成像|
