## 论文名称
Generating Sentences from a Continuous Space

## 论文作者
*Samuel R. Bowman, NLP Group and Dept. of Linguistics Stanford University
*Luke Vilnis, CICS, University of Massachusetts Amherst

## 论文简介
本篇文章虽然比较老，是CoNLL 2016上的文章，但是它的一作是斯坦福大牛Bowman，这是第一篇将VAE应用于生成连续句子的文章。之前都是将文章或者句子看做bag of words。

这篇文章提出了基于RNN的VAE模型，目的是学习句子内容的全局潜在重述。框架如下：

![主题框架](https://github.com/axxash/NLP_weekly/raw/master/20181214/picture/Generating%20Sentences%20from%20a%20Continuous%20Space.png)

## 论文摘要
The standard recurrent neural network
language model (rnnlm) generates sen- tences one word at a time and does not work from an explicit global sentence rep- resentation. In this work, we introduce and study an rnn-based variational au- toencoder generative model that incorpo- rates distributed latent representations of entire sentences. This factorization al- lows it to explicitly model holistic prop- erties of sentences such as style, topic, and high-level syntactic features. Samples from the prior over these sentence repre- sentations remarkably produce diverse and well-formed sentences through simple de- terministic decoding. By examining paths through this latent space, we are able to generate coherent novel sentences that in- terpolate between known sentences. We present techniques for solving the difficult learning problem presented by this model, demonstrate its effectiveness in imputing missing words, explore many interesting properties of the model’s latent sentence space, and present negative results on the use of the model in language modeling.

## 论文下载
[下载地址](https://arxiv.org/pdf/1511.06349)

## 代码
[github代码](https://github.com/timbmg/Sentence-VAE)
