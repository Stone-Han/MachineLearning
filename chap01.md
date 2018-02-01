---

title: 机器学习笔记1
date: 2018-02-01 21:04:00
tags: [machine learning]
categories: 笔记

---

课程网址：
[http://open.163.com/movie/2008/1/M/C/M6SGF6VB4_M6SGHFBMC.html](http://open.163.com/movie/2008/1/M/C/M6SGF6VB4_M6SGHFBMC.html)

学习资料下载：
[https://cs229.stanford.edu](https://cs229.stanford.edu)

preliminaries:

- 线性代数
- 概率论
- matlab/Octave

<!-- more -->


# Machine Learning definition #

-Arthur Samuel: Filed of study that gives computers the ability to learn without being explicitly programmed.

-Tom Mitchell: A computer program is said to learn from experience E with respect to some task T and some performance measure P, if its performance on T, as measured by P, improves with experience E.

本课程主要包括下面四个方面：

# Supervised Learning #

监督学习分为两类，一类是回归（Regression），一类是分类（Classification），分别针对连续数据和离散数据。

## Regression ##

以房屋买卖为例子，我们可以根据房屋的面积和价格建立联系，然后让机器学习提供他们之间的联系，然后当我提供其他输入的时候，机器可以返回给我一个答案。

之所以称为“监督”学习，是因为我们提供了标准答案，例如上面的价格。

## Classification ##

以肿瘤为例子，我们可以搜集数据判断肿瘤是良性的或者恶性的。

##Learning Theory ##

理论的证明，比如如何证明能够将邮编的识别率达到99%。

## Unsupervised Learning ##

我们不知道正确答案，比如给一些数据，能够得到什么数据结构。
聚类问题是其中的一类。
应用：

-用一张照片构建3D模型，wow
-Cocktail party problem (从party上所有说话的人中提取你感兴趣的那个人）


##  Reinforcement Learning ##

强化学习主要用在不需要进行一次决策的领域。比如在利用监督学习进行肿瘤预测的时候，你只需要预测一次。但是在强化学习中，需要在一段时间内做出一系列决策。比如，我们需要做一系列好的决策才能让无人机飞起来。

强化学习的基础是回报函数（reward function）。比如，狗狗做了好事，你会夸奖他"good dog"，做了坏事，你会说"bad dog"，贱贱地，他就学会了怎样做更多的好事。