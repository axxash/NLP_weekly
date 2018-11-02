### 论文题目
Convolutional Sequence to Sequence Learning

### 作者
    1.Jonas Gehring 
    2.Michael Auli 
    3.David Grangier 
    4.Denis Yarats 
    5.Yann N.Dauphin 
    Facebook AI Research

### 摘要
The prevalent approach to sequence to sequence learning maps an input sequence to a variable length output sequence via recurrent neural net- works. We introduce an architecture based en- tirely on convolutional neural networks.1 Com- pared to recurrent models, computations over all elements can be fully parallelized during training to better exploit the GPU hardware and optimiza- tion is easier since the number of non-linearities is fixed and independent of the input length. Our use of gated linear units eases gradient propaga- tion and we equip each decoder layer with a sep- arate attention module. We outperform the accu- racy of the deep LSTM setup ofWu et al. (2016) on both WMT’14 English-German and WMT’14 English-French translation at an order of magni- tude faster speed, both on GPU and CPU.

### 推荐理由
这篇论文是由facebook AI团队提出，其设计了一种完全基于卷积神经网络的模型，应用于seq2seq任务中。在机器翻译任务上比以往效果更好，同时大大提高了运行速度。

将CNN成功应用于seq2seq任务中，发挥了CNN并行计算和层级结构的优势，CNN的并行计算明显提高了运行速度，同时CNN的层级结构方便模型发现句子中的结构信息。模型中的一些细节处理，比如非线性部分采用的是门控结构 gated linear units（GLM），多跳注意机制multi-hop attention，都是模型效果提升的关键。

目前Facebook已经在github上开源了相关代码(基于Pytorch实现)，并整合在了Facebook的开源项目[fairseq](https://github.com/pytorch/fairseq)中，其中还包括Facebook其他的一些工作。

### 论文地址
[PDF下载](http://cslt.riit.tsinghua.edu.cn/mediawiki/images/b/bb/Cnn_seq2seq.pdf)
