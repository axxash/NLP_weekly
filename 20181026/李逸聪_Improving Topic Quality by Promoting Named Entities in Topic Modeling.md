###论文名称
Improving Topic Quality by Promoting Named Entities in Topic Modeling

###论文作者
Katsizryna Krasnashchok, Salim Jouili. Both of them are from EURA NOVA.

###论文简介
本篇论文发表在ACL 2018上，它的想法是，将命名实体引入LDA，提高了聚类结果的质量。具体通过两种方法：1. 对于doc-word的矩阵，如果该列是命名实体，本列乘以\alpha。2. 对于doc-word的矩阵，如果该列是命名实体，本列加上本行最大的词频。在实验结果上，比2013年的一篇将命名实体引入LDA的效果好。

###论文摘要
News-related content has been extensively studied in both topic modeling research and named entity recognition. However, expressive power of named entities and their potential for improving the quality of
discovered topics has not received much attention. In this paper we use named entities as domain-specific terms for newscentric content and present a new weighting model for Latent Dirichlet Allocation. Our experimental results indicate that involving more named entities in topic descriptors positively influences the overall quality of topics, improving their interpretability, specificity and diversity.

###论文下载
[Improving Topic Quality by Promoting Named Entities in Topic Modeling下载](http://aclweb.org/anthology/P18-2040)

