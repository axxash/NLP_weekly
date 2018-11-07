### 论文题目
Annotation Artifacts in Natural Language Inference Data

### 作者
    1.Suchin Gururangan
    2.Swabha Swayamdipta
    3.Omer Levy
    4.Roy Schwartz
    5.Samuel R. Bowman
    6.Noah A. Smith

### 摘要
Large-scale datasets for natural language inference are created by presenting crowd workers with a sentence (premise), and asking them to generate three new sentences (hypotheses) that it entails, contradicts, or is logically neutral with respect to. We show that, in a significant portion of such data, this protocol leaves clues that make it possible to identify the label by looking only at the hypothesis, without observing the premise. Specifically, we show that a simple text categorization model can correctly classify the hypothesis alone in about 67% of SNLI (Bowman et. al, 2015) and 53% of MultiNLI (Williams et. al, 2017). Our analysis reveals that specific linguistic phenomena such as negation and vagueness are highly correlated with certain inference classes. Our findings suggest that the success of natural language inference models to date has been overestimated, and that the task remains a hard open problem.

### 推荐理由
该论文是发表在NAACL 2018上的一篇short paper，第一作者 Suchin Gururangan 来自华盛顿大学语言系，其余作者包括 Omer Levy、Sam Bowman、Noah Smith 等知名学者。本文提出一个值得讨论的问题：自然语言推理（NLI）数据在构造的过程中存在一系列的人工模式，这种模式的直接后果是模型可以在不需要知道推理前提（premise）的条件下就可以以 67%的准确率判断推理假设（hypothesis）是否是蕴含（entailment）中立（neural）或对立（contradiction）。文中值得关注的地方包括：如何分析数据，发掘其中的人工模式；如何在发掘了人工模式的基础上重新审视现有模型。另外，一个更泛化的问题是：我们的模型是真的完成我们对于相应任务的目标，还是在单纯「玩弄」数据？

### 论文地址
[PDF下载](https://arxiv.org/pdf/1803.02324)
