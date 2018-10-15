论文题目：Dynamic and Static Topic Model for Analyzing Time-Series Document Collections

论文作者：Rem Hida, Naoya Takeishi, Takehisa Yairi, Koichi Hori；作者均来自东京大学航天航空系，其中2作同时来自RIKEN高级情报中心。

该论文发表在ACL 2018上，是一篇5页的短文。

本文提出了一个动静态主题模型，它同时考虑了存在时间主题变化的动态结构和某一时间下的主题层次的静态结构。这两个结构分别是这样的，
作者用topic-word分布与前一个epoch的topic-word分布的加权来模拟分布的时间演变；
而静态结构是，在原有的lda基础上，topic distribution后 加一个subtopic distribution。

具体是这样的，对于dynamic structure有个/phi_{t}Dirichlet(weight*/phi_{t-1})的分布。
其中weight是权重，/phi_{t}是第t个时刻的word-topic分布，/phi_{t-1}是第t-1时刻的word-topic分布。
对于static structure的每一个epoch，它的生成模型过程是，
对于每个subtopic，生成一个topic-word分布，就是前面说的那个分布。对于每个doc，生成一个supertopic分布，对于每一个supertopic，生成一个subtopic分布。
对于每个单词，生成一个supertopic-word assignment，subtopic-word assignment, word-observation。
推断方式是在随机EM的基础上再次进行了近似（用的MDTM中的方式）。


推荐理由：
1. 简单的思想发了ACL，我觉得它的表达清晰占了优势。写作能力很重要。
2. 结合了动态和静态的分类，比较新颖。

优点：
1. 本文叙述非常清楚。文章长度较短，通过一系列连词的表达，叙述非常清晰得体。主要是最近读了同学写的文章草稿，有很明显的比较。

缺点：
1. inference时，在随机EM方法的基础上再次进行了近似，不是很准确。但是在实验中，与LDA,PAM,DRTM比较，本文得到了最好的perplexity。不过，比较的这些都是比较老的算法。
