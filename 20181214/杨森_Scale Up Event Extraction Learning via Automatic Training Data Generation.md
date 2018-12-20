### 论文题目
Scale Up Event Extraction Learning via Automatic Training Data Generation

### 来源
AAAI 2018

### 作者
    1.Ying Zeng 
    2.Yansong Feng 
    3.Rong Ma 
    4.Zheng Wang 
    北大和中科院
    
### 摘要
The task of event extraction has long been investigated in a supervised learning paradigm, which is bound by the num- ber and the quality of the training instances. Existing training data must be manually generated through a combination of expert domain knowledge and extensive human involvement. However, due to drastic efforts required in annotating text, the resultant datasets are usually small, which severally affects the quality of the learned model, making it hard to general- ize. Our work develops an automatic approach for generating training data for event extraction. Our approach allows us to scale up event extraction training instances from thousands to hundreds of thousands, and it does this at a much lower cost than a manual approach. We achieve this by employ- ing distant supervision to automatically create event anno- tations from unlabelled text using existing structured knowl- edge bases or tables. We then develop a neural network model with post inference to transfer the knowledge extracted from structured knowledge bases to automatically annotate typed events with corresponding arguments in text. We evaluate our approach by using the knowledge extracted from Freebase to label texts from Wikipedia articles. Experimental results show that our approach can generate a large number of high- quality training instances. We show that this large volume of training data not only leads to a better event extractor, but also allows us to detect multiple typed events.
Introduction

### 推荐理由
本文主要包括两部分的内容，事件生成和事件抽取。基于freebase生成事件元信息，然后利用远程监督生成事件语句。基于事件的关键角色识别事件类型。但事件抽取采用的数据集是第一步生成的事件数据。

### 论文地址
[PDF下载](http://cn.arxiv.org/pdf/1712.03665.pdf)
