# 骐骥团队-26冬令营-模型组（初级）学习报告

## 1. 概览
基于 `骐骥团队-26冬令营-模型组.pdf` 中“初级组”的学习要求，在本报告中总结了寒假期间的学习成果。学习内容覆盖了 PyTorch 基础操作、机器学习基础算法、神经网络核心概念以及卷积神经网络（CNN）的应用。  

由于提供的[GitHub仓库](https://github.com/deeplearningzerotoall/PyTorch)中内容写的不是很详细，因此在学习过程中，我参考了其他的学习资源，并总结成相关[学习笔记]在 `Notes` 目录中。

所有代码文件均已整理在 `Notes` 和 `Notes 2` 目录中，以下是详细的学习内容与文件对应关系。

---

## 2. 机器学习与 PyTorch 基础 (Machine Learning & PyTorch Basics)
本部分主要对应“初级组”要求的前半部分，涵盖 Tensor 操作、线性回归、逻辑回归及分类任务。

### 2.1 张量操作与基础 (Tensor Manipulation)
- **[Lab-01-1 Tensor Manipulation 1](./Notes%202/机器学习与PyTorch基础/Lab-01-1%20Tensor%20Manipulation%201.ipynb)**
  - 学习了 PyTorch 张量的基本创建、属性查看。
- **[2.Pytorch张量](./Notes/2.Pytorch张量.ipynb)**
  - 深入学习了张量的高级操作与数学运算。

### 2.2 线性回归 (Linear Regression)
- **[Lab-02 Linear Regression](./Notes%202/机器学习与PyTorch基础/Lab-02_linear_regression.ipynb)**
  - 实现了单变量线性回归模型。
- **[Lab-04-1 Multivariable Linear Regression](./Notes%202/机器学习与PyTorch基础/Lab-04_1_multivariable_linear_regression.ipynb)**
  - 扩展至多变量线性回归。

### 2.3 分类任务 (Classification)
- **[Lab-05 Logistic Regression](./Notes%202/机器学习与PyTorch基础/Lab-05_logistic_classification.ipynb)**
  - 学习了二分类问题的逻辑回归实现。
- **[Lab-06 Softmax Classification](./Notes%202/机器学习与PyTorch基础/Lab-06_1_softmax_classification.ipynb)**
  - 学习了多分类问题的 Softmax 回归实现。

### 2.4 数据加载与训练技巧 (Data Loading & Tips)
- **[Lab-04-2 Loading Data](./Notes%202/机器学习与PyTorch基础/Lab-04_2_load_data.ipynb)**
  - 掌握了使用 `Dataset` 和 `DataLoader` 进行批量数据加载的方法。
  - 相关数据文件：`Notes 2/机器学习与PyTorch基础/data-*.csv`
- **[Lab-07-1 Tips](./Notes%202/机器学习与PyTorch基础/lab-07_1_tips.ipynb)**
  - 学习了训练过程中的实用技巧。
- **[Lab-07-2 MNIST Introduction](./Notes%202/机器学习与PyTorch基础/Lab-07_2_mnist_introduction.ipynb)**
  - 初步接触 MNIST 数据集与简单的分类模型训练。

---

## 3. 神经网络基础与分类任务 (Neural Network Basics & Classification)
本部分深入神经网络的核心组件，对应要求中的 Lab-08 至 Lab-09 系列。

### 3.1 感知机与多层感知机 (Perceptron & MLP)
- **[1.神经网络与模型训练](./Notes/1.神经网络与模型训练.ipynb)**
  - 系统学习了神经网络的基本结构与训练流程。
- **[3.使用Pytorch构建神经网络](./Notes/3.使用Pytorch构建神经网络.ipynb)**
  - 掌握了使用 `torch.nn.Sequential` 和 `class` 方式构建模型。

### 3.2 激活函数与损失函数
- **[4.常用激活函数和损失函数详解](./Notes/4.常用激活函数和损失函数详解.ipynb)**
  - 详细分析了 Sigmoid, Tanh, ReLU 等激活函数及 MSE, CrossEntropy 等损失函数。

### 3.3 优化与正则化 (Optimization & Regularization)
- **[6.神经网络性能优化技术](./Notes/6.神经网络性能优化技术.ipynb)**
  - 综合介绍了提升模型性能的策略。
- **[8.批归一化](./Notes/8.批归一化.ipynb)** (对应 Lab-09-4)
  - 实现了 Batch Normalization，理解其加速收敛的作用。
- **[9.学习率优化](./Notes/9.学习率优化.ipynb)**
  - 探讨了学习率对训练的影响及调度策略。
- **[10.过拟合及其解决方法](./Notes/10.过拟合及其解决方法.ipynb)** (对应 Lab-09-3 Dropout)
  - 学习了 Dropout 等防止过拟合的技术。
- **[7.批大小对神经网络性能的影响](./Notes/7.批大小对神经网络性能的影响.ipynb)**
  - 实验分析了不同 Batch Size 的影响。

---

## 4. 神经网络与卷积神经网络 (Neural Networks & CNN)
本部分涵盖计算机视觉核心内容，对应要求中的 Lab-10 系列。

### 4.1 计算机视觉基础
- **[5.计算机视觉基础](./Notes/5.计算机视觉基础.ipynb)**
  - 介绍了图像处理的基础知识。
- **[11.卷积神经网络](./Notes/11.卷积神经网络.ipynb)** (对应 Lab-10-0/1/2)
  - 深入学习了卷积层、池化层及其在 CNN 中的应用。

### 4.2 高级 CNN 技术与应用
- **[12.数据增强](./Notes/12.数据增强.ipynb)** (对应 Lab-10-4)
  - 学习了多种图像增强技术以提升模型鲁棒性。
- **[15.基于ResNet模型实现猫狗分类](./Notes/15.基于ResNet模型实现猫狗分类.ipynb)** (对应 Lab-10-5/6/7)
  - **实战项目**：基于 ResNet 模型实现了猫狗图像分类。
  - 涵盖了 ResNet 结构、迁移学习应用及完整训练流程。
- **[14.迁移学习](./Notes/14.迁移学习.ipynb)**
  - 专门探讨了如何利用预训练模型解决新问题。
- **[13.类激活图](./Notes/13.类激活图.ipynb)**
  - 学习了 CAM 技术，实现了模型预测的可视化解释。

---

## 5. 总结与反思

### 5.1 学习策略与成果
本次寒假学习是我初次系统性接触深度学习与 PyTorch 框架。鉴于时间有限且作为初学者，我采取了**“先速通，再深入研究”**的学习策略 *~~（但是好像还不能做到很多概念和细节都理解清楚）~~*。

通过这段时间的集中学习，我已经能够独立跑通从数据加载、模型构建、训练到推理的完整流程，并成功完成了线性回归、基础分类以及 ResNet 猫狗分类等实战项目，对网上流传的深度学习 ***~~“炼丹”~~*** 过程有了直观的认识。

### 5.2 待加强之处
但是由于采取了速通策略，目前对部分细节的理解还停留在感性认识层面，尚未完全吃透：
- **数学原理**：对梯度下降、反向传播等算法背后的数学推导（如链式法则的具体计算）还不够熟练。
- **模型调优**：目前的模型训练更多是基于现有结构，对于如何针对特定问题自主设计网络结构或进行精细化的超参数调优，还不太会。
- **代码细节**：相关代码在没有参照的情况下没有办法独立写出来

### 5.3 未来展望
接下来的学习中，我计划回头复盘，重点攻克上述薄弱环节，继续夯实基础，努力实现从“会用”向“懂原理”的进步。

## 6. 附件

- **模型权重**: `Notes/fashion_mlp.pth` (保存的模型参数)
- **数据集**:
  - `data/FashionMNIST`
  - `data/MNIST`
  - `data/cat&dog`
- **图片资源**: `Images/` 目录包含约 40 张用于笔记说明的 PNG 图片。
- **参考资料**: `骐骥团队-26冬令营-模型组.pdf`

---
