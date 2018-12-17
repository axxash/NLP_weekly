## 论文题目
Adversarial Network Embedding
## 作者
Quanyu Dai, Qiang Li, Jian Tang, Dan Wang 
Department of Computing, The Hong Kong Polytechnic University, Hong Kong
School of Software, FEIT, The University of Technology Sydney, Australia
HEC Montreal, Canada
Montreal Institute for Learning Algorithms, Canada
## 发表会议
AAAI2018
## 摘要
学习网络的低维表示已经证明在各种任务中是有效的，例如节点分类，链路预测和网络可视化。现有方法可以有效地将不同的结构属性编码成表示，例如邻域连接模式，全局结构角色相似性和其他高阶邻近性。然而，除了捕获网络结构属性的目标之外，它们中的大多数都缺乏用于增强表示的稳健性的额外约束。在本文中，我们的目标是利用生成对抗网络的优势捕获潜在特征，并研究其在学习稳定和健壮的图形表示方面的贡献。具体而言，我们提出了一种对抗性网络嵌入（ANE）框架，该框架利用对抗性学习原则来规范表征学习。它由两个部分组成，即结构保持组件和对抗性学习组件。前一个组件旨在捕获网络结构属性，而后一个组件通过将潜在表示的后验分布与给定先验相匹配，有助于学习稳健表示。
## 论文下载地址
[论文](https://arxiv.org/abs/1711.07838)点击下载
## 推荐理由
本文使用ＧＡＮ增强了ＮＥ表示学习的鲁棒性和稳定性．对抗性学习组件中的判别器是将高斯噪声作为正样本，那么生成器产生的embeddings理论上就会越来越接近高斯分布，也就是说没有太强的特征性，这样就相当于增强了其鲁棒性．在结构保持组件里面，有目标生成器函数和上下文生成器函数，分别用于将目标点和上下文点表示成向量，同时这个目标生成器函数也是后面对抗学习组件里面的生成器函数．
