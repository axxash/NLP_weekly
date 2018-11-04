## 论文名称
Incorporating Knowledge Graph Embeddings into Topic Modeling

## 论文作者
Liang Yao, Yin Zhang,* Baogang Wei, Zhe Jin, Rui Zhang, Yangyang Zhang, Qinfei Chen.

All of them are from Zhejiang University.

## 论文简介
本篇论文发表在AAAI 2017上。它提出了一种新的基于知识的主题模型，将知识图谱嵌入到LDA中。算法具体是：在原有的LDA算法基础上，添加了最后一步，对于每个链接到已存在的知识图谱的实体，进行采样。最后在20NG，NIPS，Ohsumed数据集上进行了测试，比LDA算法的coherence高（评测标准是PMI）。

## 论文摘要
Probabilistic topic models could be used to extract lowdimension topics from document collections. However, such
models without any human knowledge often produce topics that are not interpretable. In recent years, a number
of knowledge-based topic models have been proposed, but
they could not process fact-oriented triple knowledge in
knowledge graphs. Knowledge graph embeddings, on the
other hand, automatically capture relations between entities
in knowledge graphs. In this paper, we propose a novel
knowledge-based topic model by incorporating knowledge
graph embeddings into topic modeling. By combining latent
Dirichlet allocation, a widely used topic model with knowledge encoded by entity vectors, we improve the semantic coherence significantly and capture a better representation of
a document in the topic space. Our evaluation results will
demonstrate the effectiveness of our method.
## 论文下载
[Incorporating Knowledge Graph Embeddings into Topic Modeling下载](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/download/14170/14086)

