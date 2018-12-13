### 论文题目
Improved Variational Autoencoders for Text Modeling using Dilated Convolutions

### 作者
Zichao Yang, Zhiting Hu, Ruslan Salakhutdinov, Taylor Berg-Kirkpatrick

Carnegie Mellon University

ICML 2017

###  摘要
Recent work on generative text modeling has found that variational autoencoders (VAE) with LSTM decoders perform worse than simpler LSTM language models (Bowman et al., 2015). This negative result is so far poorly understood, but has been attributed to the propensity of LSTM decoders to ignore conditioning informa- tion from the encoder. In this paper, we ex- periment with a new type of decoder for VAE: a dilated CNN. By changing the decoder’s di- lation architecture, we control the size of con- text from previously generated words. In ex- periments, we find that there is a trade-off be- tween contextual capacity of the decoder and ef- fective use of encoding information. We show that when carefully managed, VAEs can outper- form LSTM language models. We demonstrate perplexity gains on two datasets, representing the first positive language modeling result with VAE. Further, we conduct an in-depth investigation of the use of VAE (with our new decoding archi- tecture) for semi-supervised and unsupervised la- beling tasks, demonstrating gains over several strong baselines.

### 推荐理由
这是发表在ICML 2017上的一篇文章。本文主要工作是以dilated CNN作为传统的VAE的解码器。
并在几个数据集上应用了，比LSTM语言模型效果好（这里是因为2015年Bowman等人发现，用
LSTM作为解码器，效果比LSTM语言模型差，所以在本文中用这个作为比较对象）。

另外，作者还在这个框架上对半监督以及无监督任务做了实验。

### 论文地址
[PDF 下载](http://proceedings.mlr.press/v70/yang17d/yang17d.pdf)