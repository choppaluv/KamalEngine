<div  align="center">  
<img src="docs/kae-logo-light.png" width = "30%" height = "30%" alt="icon"/>  
</div>

# KAmalEngine

KAmalEngine is a software system that implements Knowledge Amalgamation algorithms. In knowledge amalgamation, we use trained deep network models available online to do a model-reusing task. Given multiple pretrained teacher networks, which specializes in different vision problems, the goal of knowledge amalgamation is to learn a lightweight student model capable of handling the comprehensive tasks, without human-labeled annotations. It is written in Python and powered by the Pytorch deep learning framework.

## Table of contents
   * [Introduction](#Introduction)
   * [Algorithms](#Algorithms)
   * [Help](#help)

## Introduction

The goal of KamalEngine is to provide a high-quality, high-performance code framework for Knowledge Amalgamation *research*. For more extensive discussions about Knowledge Amalgamation, please see the [AAAI 2019 paper](https://arxiv.org/abs/1811.02796v1). This respository focuses on designed a flexible code framework in order to support rapid implementation and evaluation of novel research. KamalEngine includes implementations of the following Knowledge Amalgamation algorithms:
- [Amalgamating Knowledge towards Comprehensive Classification](https://arxiv.org/abs/1811.02796v1) -- *AAAI 2019*
- [Student Becoming the Master: Knowledge Amalgamation for Joint Scene Parsing, Depth Estimation, and More](https://arxiv.org/abs/1904.10167) -- *CVPR 2019*
- [Knowledge Amalgamation from Heterogeneous Networks by Common Feature Learning](http://arxiv.org/abs/1906.10546) -- *IJCAI 2019*
- [Amalgamating Filtered Knowledge: Learning Task-customized Student from Multi-task Teachers](https://arxiv.org/abs/1905.11569) -- *IJCAI 2019*
- [Customizing student networks from heterogeneous teachers via adaptive knowledge amalgamation]() (Comming soon) -- *ICCV 2019*


## Algorithms
This repo provides some algorithms of KA.


### Student Becoming the Master
Knowledge amalgamation for multiple teachers by feature projection.  
[Student Becoming the Master: Knowledge Amalgamation for Joint Scene Parsing, Depth Estimation, and More](https://arxiv.org/abs/1904.10167) -- *CVPR 2019*  
![sbm-demo](examples/sbm/demo.png)

### Common Feature Learning
Extract common features from multiple teacher models.  
[Knowledge Amalgamation from Heterogeneous Networks by Common Feature Learning](http://arxiv.org/abs/1906.10546) -- *IJCAI 2019*

Feature Space             |  Common Space
:-------------------------:|:-------------------------:
![cfl-feature-space](examples/cfl/tsne_results/feature_space_tsne_0.png)  |  ![cfl-feature-space](examples/cfl/tsne_results/common_space_tsne_0.png)

### Amalgamating Knowledge towards Comprehensive Classification
Layer-wise amalgamation  
[Amalgamating Knowledge towards Comprehensive Classification](https://arxiv.org/abs/1811.02796v1) -- *AAAI 2019*  
![layerwise-ka-framework](examples/layer_wise_ka/layerwise-ka-framework.png)

### Customizing student networks from heterogeneous teachers via adaptive knowledge amalgamation (In Progress)
![adaptive-ka-framework](examples/adaptive_ka/adaptive-ka-framework.jpg)

### Recombination
Build a new multi-task model by combining&pruning weight matrixs from distinct-task teachers.
![recombination-framework](examples/recombination/recombination-framework.png)

### Amalgamating Filtered Knowledge
Amalgamate knowledge from a pool of multi- or single-task teachers working on different tasks. The TargetNet after training, at a reasonably compact size, handles multiple customized tasks.

<div  align="center">  
<img src="examples/afk/targetnet.png" width = "400" alt="icon"/>  
</div>

## Help
For more information, see `docs` and `examples`

## Authors
| | |
|:--------------:|:-----:|
[Gongfan Fang](https://github.com/VainF) | fgfvain97@zju.edu.cn  
[Yixin Ji](https://github.com/Ssssseason) | jiyixin@zju.edu.cn  
[Yanling Yin](https://github.com/ylyinzju) | yanlingyin@zju.edu.cn  
[Jingwen Ye]() | yejingwen@zju.edu.cn  
[Sihui Luo]() | sihuiluo829@zju.edu.cn  
[Chengchao Shen]() | chengchaoshen@zju.edu.cn  
[Mengqi Xue]() | mqxue@zju.edu.cn  

[Homepage of VIPA Group](https://www.vipazoo.cn/index_en.html), Zhejiang University, China

<div  align="left">  
<img src="docs/vipa-logo.png" width = "40%" height = "40%" alt="icon"/>  
</div>

## Citation
```
@inproceedings{shen2019amalgamating,
  author={Shen, Chengchao and Wang, Xinchao and Song, Jie and Sun, Li and Song, Mingli},
  title={Amalgamating Knowledge towards Comprehensive Classification},
  booktitle={AAAI Conference on Artificial Intelligence (AAAI)},
  pages={3068--3075},
  year={2019}
}
```

```
@inproceedings{ye2019student,
  title={Student Becoming the Master: Knowledge Amalgamation for Joint Scene Parsing, Depth Estimation, and More},
  author={Ye, Jingwen and Ji, Yixin and Wang, Xinchao and Ou, Kairi and Tao, Dapeng and Song, Mingli},
  booktitle={Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition},
  pages={2829--2838},
  year={2019}
}
```

```
@inproceedings{luo2019knowledge,
  title={Knowledge Amalgamation from Heterogeneous Networks by Common Feature Learning},
  author={Luo, Sihui and Wang, Xinchao and Fang, Gongfan and Hu, Yao and Tao, Dapeng and Song, Mingli},
  booktitle={Proceedings of the 28th International Joint Conference on Artificial Intelligence (IJCAI)},
  year={2019},
}
```

```
@inproceedings{shen2019customizing,
  author={Shen, Chengchao and Xue, Mengqi and Wang, Xinchao and Song, Jie and Sun, Li and Song, Mingli},
  title={Customizing student networks from heterogeneous teachers via adaptive knowledge amalgamation},
  booktitle={The IEEE International Conference on Computer Vision (ICCV)},
  year={2019}
}
```

```
@inproceedings{Ye_Amalgamating_2019,
  year={2019},
  author={Ye, Jingwen and Wang, Xinchao and Ji, Yixin and Ou, Kairi and Song, Mingli},
  title={Amalgamating Filtered Knowledge: Learning Task-customized Student from Multi-task Teachers}
  booktitle={Proceedings of the 28th International Joint Conference on Artificial Intelligence (IJCAI)},
  year={2019},
}
```