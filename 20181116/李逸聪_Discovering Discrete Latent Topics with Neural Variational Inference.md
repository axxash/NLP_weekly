## 论文名称
Discovering Discrete Latent Topics with Neural Variational Inference

## 论文作者
Yishu Miao 1 Edward Grefenstette 2 Phil Blunsom 1 2

1 University of Oxford, UK
2 DeepMind, London, UK

## 论文简介
本篇论文发表在ICML 2017上。通过Neural Variational Inference的方法，进行文本主题聚类，并在MXM Song Lyrics, 20NewsGroups and Reuters News上进行了实验，perplexity比OnlineLDA, NVLDA, HDP小。另外，还比较了在不同init topics时，recurrent stick breaking construction的perplexity，发现越大越好。最后比较了topic coherence，作者提出的三个model效果都比较好。

具体的，作者在LDA模型基础上，将topic distribution和topic assignment过程替换为了gaussian process。即，x～N(μ，σ)，θ=g(x)。这里的N是高斯分布，至于g函数，作者提出了三种方法。1是g为softmax函数，θ = softmax(Wx)，2是引入了stick-breaking构造，θ = fSB(sigmoid(Wx))，其中FSB是stick-breaking的计算函数，3是引入了神经网络，θ = fSB(fRNN(x))，其中FRNN是rnn网络。由于RNN能够不断动态的生成新的logits来break the stick，所以这样看来，这种方法是可以训练无穷个topic的。

## 论文摘要
Topic models have been widely explored as probabilistic generative models of documents. Traditional inference methods have sought closedform derivations for updating the models, however as the expressiveness of these models grows,
so does the difficulty of performing fast and
accurate inference over their parameters. This
paper presents alternative neural approaches to
topic modelling by providing parameterisable
distributions over topics which permit training
by backpropagation in the framework of neural variational inference. In addition, with the
help of a stick-breaking construction, we propose a recurrent network that is able to discover a notionally unbounded number of topics, analogous to Bayesian non-parametric topic
models. Experimental results on the MXM
Song Lyrics, 20NewsGroups and Reuters News
datasets demonstrate the effectiveness and efficiency of these neural topic models.

## 论文下载
[Discovering Discrete Latent Topics with Neural Variational Inference下载](https://arxiv.org/pdf/1706.00359)
