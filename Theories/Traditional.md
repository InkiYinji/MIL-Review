[上一级](TheoriesREADME.md)

---

传统MIL方法大致分为三种：
1. **实例方法**：首先预测实例标签，并通过MIL假设计算包标签；
2. **包方法**：设计类似于高斯核的MIL包距离度量，使得$k$NN和SVM等基于距离矩阵的方法得以施展；
3. **嵌入方法**：将包转换为向量，使得传统机器学习策略生效，这也是目前MIL表征学习的基础；

当然，立足于深度MIL方法的小伙伴只需大致了解这类方法。以下是对一些经典方法的归类：


|方法名|                                         团队                                         |期刊/会议|全称|思想|领域|
|:--------------------:|:----------------------------------------------------------------------------------:|:---:|:---:|:---:|:---:|
|MINTL|  [广东工业大学](https://scholar.google.com/citations?user=ZF3gp9wAAAAJ&hl=zh-CN&oi=sra)  |TNNLS'24|Multi-instance nonparallel tube learning|基于优化理论的类边界信息学习，以提升模型性能|理论
|[ISK](https://inkiyinji.blog.csdn.net/article/details/112124291)|                     [周志华](http://129.211.169.156/publication)                      |KDD‘19|[Isolation set-kernel and its application to multi-instance learning](https://inkiyinji.blog.csdn.net/article/details/105624719)|基于孤立核设置集合核和嵌入函数|理论
|[MILDM](https://github.com/InkiInki/MILDM-MNIST)|  [悉尼科技大学](https://scholar.google.com/citations?user=kbnFw94AAAAJ&hl=zh-CN&oi=sra)  |TKDE'18|[Multi-instance Learning with discriminative bag mapping](https://inkiyinji.blog.csdn.net/article/details/108139662)|利用辨别性优化嵌入结果|理论
|[miVLAD](http://www.lamda.nju.edu.cn/code_SMIL.ashx)|                     [周志华](http://129.211.169.156/publication)                      |TNNLS'16|[Scalable algorithms for multi-instance learning](https://inkiyinji.blog.csdn.net/article/details/106600849)|基于$k$Means聚类的高效MIL算法|理论
|[miFV](http://www.lamda.nju.edu.cn/code_SMIL.ashx)|                     [周志华](http://129.211.169.156/publication)                      |ICDM'14|[Scalable multi-instance learning](https://inkiyinji.blog.csdn.net//article/details/106419932)|混合高斯模型及Fisher核编码包为向量|理论
|[BAMIC](https://github.com/InkiInki/BAMIC-MNIST)|                     [周志华](http://129.211.169.156/publication)                      |Applied Intelligence'09|[Multi-instance clustering with applications to multi-instance prediction](https://blog.csdn.net/Knight_ZJY/article/details/127075256)|利用包距离度量和$k$Means聚类获取包嵌入向量|理论