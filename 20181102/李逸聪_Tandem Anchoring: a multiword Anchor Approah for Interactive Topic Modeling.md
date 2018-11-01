## 论文名称
Tandem Anchoring: a multiword Anchor Approah for Interactive Topic Modeling

## 论文作者
* Jeffery Lund, Connor Cook, Kevin Seppi. All of them are from Computer Science Department of Brigham Young University.
* Jordan Boyd-Graber is from Computer Science Department of University of Colorado Boulder.

## 论文简介
本篇论文发表在ACL 2017上。本文面向的是interactive work，要求速度快，需要用到先验知识提升效果，anchor正好有这两种优势。同时，作者提出了多anchor的topic modeling，比传统的single anchor效果好。

```
How to find anchor word:

Low-to-mid frequency words are often anchors because anchor words must be unique to a topic; 
intuitive or high-frequency words cannot be anchors if they have probability in any other topic.
```

## 论文摘要
Interactive topic models are powerful tools
for understanding large collections of text.
However, existing sampling-based interactive topic modeling approaches scale
poorly to large data sets. Anchor methods, which use a single word to uniquely
identify a topic, offer the speed needed for
interactive work but lack both a mechanism to inject prior knowledge and lack
the intuitive semantics needed for userfacing applications. We propose combinations of words as anchors, going beyond
existing single word anchor algorithms—
an approach we call “Tandem Anchors”.
We begin with a synthetic investigation of
this approach then apply the approach to
interactive topic modeling in a user study
and compare it to interactive and noninteractive approaches. Tandem anchors
are faster and more intuitive than existing
interactive approaches.

## 论文下载
[Tandem Anchoring: a multiword Anchor Approah for Interactive Topic Modeling下载](http://aclweb.org/anthology/P17-1083)
