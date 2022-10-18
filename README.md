# rethinking_bottleneck_design_paddlepaddle

## 目录

- [1. 简介](#1-简介)
- [2. 数据集和复现精度](#2-数据集和复现精度)
- [3. 准备数据与环境](#3-准备数据与环境)
    - [3.1 准备环境](#31-准备环境)
    - [3.2 准备数据](#32-准备数据)
    - [3.3 准备模型](#33-准备模型)
- [4. 开始使用](#4-开始使用)
    - [4.1 模型评估](#41-模型评估)
    - [4.2 TIPC基础链条测试](#42-tipc基础链条测试)
- [5. LICENSE](#5-license)
- [6. 参考链接与文献](#6-参考链接与文献)


## 1. 简介
这是对论文Daquan, Zhou, et al. "Rethinking Bottleneck Structure for Efficient Mobile Network Design."的paddlepaddle复现，
在此非常感谢 `zhoudaquan` `Qibin (Andrew) Hou`等人贡献的[rethinking_bottleneck_design](https://github.com/zhoudaquan/rethinking_bottleneck_design)，提高了本repo复现论文的效率。
- 论文: Daquan, Zhou, et al. "Rethinking Bottleneck Structure for Efficient Mobile Network Design." arXiv preprint arXiv:2007.02269 (2020). [[arXiv](https://arxiv.org/abs/2007.02269)]

- 论文介绍：
 - 作者重新考虑了轻量化网络设计中逆残差网络的设计，考虑到其中的不合理，提出了一种新的sandglass模块，实验证明优于逆残差结构并且能够作为基础模型在结构搜索DARTS中取得进一步的性能提升和模型轻量化。
 
- 参考repo: [rethinking_bottleneck_design](https://github.com/zhoudaquan/rethinking_bottleneck_design)

## 2. 数据集和复现精度和评价指标

repo用到的数据集是imagenet数据集的验证集，具体参见：

- 数据集大小：

- 数据集下载链接：

- 数据格式：

  > """
  >
  > ├─imgs
  >
  >     ├──ILSVRC2012_val_00000001.JPEG
  >
  >     ├──ILSVRC2012_val_00000002.JPEG
  >
  > └─val_list.txt
  >
  > """

复现精度：

|                  |    环境(env)     |    精度（acc） | 延迟(latency)   |
| ---------------  | --------------- | -------------- | -------------- |

![image]()
## 3. 准备数据与环境

### 3.1 准备环境

使用硬件和框架版本等环境的要求如下：

- 硬件：Nvidia Tesla v100 16G x1
- 框架：
  - PaddlePaddle >= 2.3.1

库安装：

- PaddlePaddle：建议参照[Paddle官方页面](https://www.paddlepaddle.org.cn/install/quick?docurl=/documentation/docs/zh/install/pip/linux-pip.html)安装，或执行以下命令：

```shell
python -m pip install paddlepaddle-gpu==2.3.1 -i https://mirror.baidu.com/pypi/simple
```

- 其余库：

AI-Studio都有安装，可直接使用。或执行：
```shell
pip install -r requirements.txt
```

### 3.2 准备数据

可参见2中数据格式，将自定义数据集按照该格式整理即可使用。

### 3.3 准备模型

- 预训练模型(paddle)：
- 原repo提供的pytorch模型：
- 模型转换：执行`

## 4. 开始使用

### 4.1 模型评估



日志：

### 4.2 TIPC基础链条测试

参见

## 5. LICENSE


## 6. 参考链接与文献
- [rethinking_bottleneck_design](https://github.com/zhoudaquan/rethinking_bottleneck_design)
- Daquan, Zhou, et al. "Rethinking Bottleneck Structure for Efficient Mobile Network Design." arXiv preprint arXiv:2007.02269 (2020). [[arXiv](https://arxiv.org/abs/2007.02269)]
