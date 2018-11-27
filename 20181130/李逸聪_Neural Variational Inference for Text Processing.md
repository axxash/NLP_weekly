## 论文名称
Neural Variational Inference for Text Processing

## 论文作者
Yishu Miao 1 Lei Yu 1 Phil Blunsom 1 2

1 University of Oxford, UK
2 DeepMind, London, UK

## 论文简介
本篇论文发表在ICML 2016上。它构造了一个以离散文本输入为条件的推理网络来提供变分分布。并在两个不同的任务上（生成文档建模和有监督的问题问答）验证了这个框架。在效果上，文章提到比之前发布的所有基准测试都好。

以下是建立这个推断网络的步骤：
1. Construct vector representations of the observed variables: u = fx(x), v = fy(y).
2. Assemble a joint representation: π = g(u; v).
3. Parameterise the variational distribution over the latent variable: µ = l1(π);log σ = l2(π).

fx()可以是任何类型的神经网络，g()是MLP网络，l()是线性变换。

但是在NVDM上（将该模型用于生成文档建模任务中），每篇文档都会产生µ和σ参数，导致参数过多。

在这篇文章中，网络的输入x是one-hot vector，如果用BERT进行与训练，效果可能会有所提升。


## 论文摘要
Recent advances in neural variational inference
have spawned a renaissance in deep latent variable models. In this paper we introduce a generic
variational inference framework for generative
and conditional models of text. While traditional
variational methods derive an analytic approximation for the intractable distributions over latent
variables, here we construct an inference network
conditioned on the discrete text input to provide the variational distribution. We validate this
framework on two very different text modelling
applications, generative document modelling and
supervised question answering. Our neural variational document model combines a continuous
stochastic document representation with a bagof-words generative model and achieves the lowest reported perplexities on two standard test corpora. The neural answer selection model employs a stochastic representation layer within an
attention mechanism to extract the semantics between a question and answer pair. On two question answering benchmarks this model exceeds
all previous published benchmarks.

## 论文下载
[Neural Variational Inference for Text Processing下载](https://arxiv.org/pdf/1511.06038)
