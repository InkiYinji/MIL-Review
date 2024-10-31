[上一级](README.md)

---

## 1 数据集
1. [**Camelyon16**](https://camelyon17.grand-challenge.org/)：270训练 (159正常111异常)、129测试，包含实例级别标签；
2. [**TCGA肺癌数据集**](https://portal.gdc.cancer.gov/files/608e2269-04b4-4a20-aca8-d20f36800cc3)：包含两个肺癌子数据集，分别为LUSC、LUAD，文件下载索引可以参照[DSMIL](https://github.com/binli123/dsmil-wsi/tree/master/tcga-download)；
3. **AGGC22**：前列腺切除术和活检标本的H&E染色WSI数据集，其中训练：测试=168：73，详情参见CIMIL；
4. **PANDA**：多三分类，包含实例级别标签，详情参见VINO；

- **注1**：DSMIL提供了预处理版本；
- **注2**：数据集的预处理一般可以使用[**CLAM**](https://github.com/mahmoodlab/CLAM)；
## 2 预处理器
|        方法        | ResNet18 (512)  | ViT-small (384)  | ResNet50(1024)  |  CTransPath  
|:----------------:|:---------------:|:----------------:|:---------------:|:------------:|
| CaMIL (AAAI'24)  |        √        |        √         
| CIMIL (AAAI'24)  |||        √        
|  VINO(AAAI'24)   |        √        ||
| PAMIL (CVPR'24)  |||        √        
|  WiKG (CVPR'24)  ||        √        
| IBMIL (CVPR'23)  |        √        |        √         ||        √        
|      CSMIL       |||        √        
|      AdvMIL      |||        √        
|      ProDiv      |||        √        

- **注1**：ResNet18括号后的数字表示每个区块 (patch) 提取后的维度；
## 3 WSI的分割策略
|数据集| 策略1 |策略2|策略3
|--|--|--|--|
| Camelyon16 | √ |√
|TCGA-NSCLC||√|√
