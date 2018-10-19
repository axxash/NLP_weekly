### 论文题目
Attention is all you need

### 作者
1. [Ashish Vaswani](https://ai.google/research/people/AshishVaswani)
2. Noam Shazeer
3. Niki Parmar

### 摘要
The dominant sequence transduction models are based on complex recurrent or convolutional neural networks that include an encoder and a decoder. The best performing models also connect the encoder and decoder through an attention mechanism. We propose a new simple network architecture, the Transformer, based solely on attention mechanisms, dispensing with recurrence and convolutions entirely. Experiments on two machine translation tasks show these models to be superior in quality while being more parallelizable and requiring significantly less time to train. Our model achieves 28.4 BLEU on the WMT 2014 English- to-German translation task, improving over the existing best results, including ensembles, by over 2 BLEU. On the WMT 2014 English-to-French translation task, our model establishes a new single-model state-of-the-art BLEU score of 41.0 after training for 3.5 days on eight GPUs, a small fraction of the training costs of the best models from the literature.

### 推荐理由
文章只依靠self-attention机制，不使用rnn和cnn，完成seq2seq的翻译任务，提高了并行度而且取得了state of the art的效果；虽然文章标题富有煽动性，但是文章中并未说明单纯使用attention机制是否会优于结合self-attention与cnn或者rnn模型；文章中提出的一些技术multi-head attention, position embedding以及mask attention等有较大的参考价值。

### 论文地址
[Attention is all you need PDF下载](https://papers.nips.cc/paper/7181-attention-is-all-you-need.pdf)
