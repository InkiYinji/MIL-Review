[上一级](README.md)

正和无标签学习 (PU) 的训练集中只包含正样本和无标记样本，对应的问题有叶片上的异常结冰检测、诈骗邮件检测等。考虑MIL的弱监督设置，通过添加对抗扰动的方式愚弄MIL分类器，以解释模型的脆弱性和安全性。此外，对抗防御则用于降低MIL攻击者的效能。

---
|                          方法名                           |团队|期刊/会议|全称|思想|领域|
:------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------:|:---:|:---:|:------------------------:|:---:
|[**PU-MIL-AD✳**](https://github.com/Lorenzo-Perini/PU-MIL-AD)|鲁汶大学|KDD'23|[Learning from positive and unlabeled multi-instance bags in anomaly detection](https://inkiyinji.blog.csdn.net/article/details/132333927)|在MIL中首次引入PU学习的概念，并基于VAE进行异常检测|Anomaly Detection