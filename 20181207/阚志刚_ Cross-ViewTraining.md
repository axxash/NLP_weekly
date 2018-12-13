## 文章题目
Semi-Supervised Sequence Modeling with Cross-View Training
## 简介
作者提出了交叉视图训练(Cross-View Training, CVT)，这是一种半监督学习算法，它可以改进Bi-LSTM句子编码器的表示，使用标签和未标签数据的混合。这个模型在标记示例上，使用标准的监督学习。在未标记的例子中，CVT teaches辅助预测模块，这些模块可以看到输入的受限视图(例如，仅是句子的一部分)，以匹配看到整个输入的完整模型的预测。由于辅助模块和完整模型共享中间表示，这反过来又改进了完整模型。
