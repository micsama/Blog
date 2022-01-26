---
title: "Ml"
date: 2021-11-30T19:58:31+08:00
draft: false
---
---
### 有监督学习 Supervised learning
>输入打过标签 **Labeled** 的内容
>
>

- 回归问题 Regression Problem
- 分类问题 Classificaion Problem
### 无监督学习 Unsupervised learning
> 输入没打标签  **unlabled**  的内容
- 聚类 
- 奇异值分解（鸡尾酒问题

## 方法
### 一：梯度下降 Gradient descent
>- 代价函数 j
>- 假设函数 h
>- 学习率 a
### 二：正规方程
梯度下降与正规方程的比较：

| 梯度下降             | 正规方程                                     |
| ---------------- | ---------------------------------------- |
| 需要选择学习率$\alpha$  | 不需要                                      |
| 需要多次迭代           | 一次运算得出                                   |
| 当特征数量$n$大时也能较好适用 | 需要计算${{\left( {{X}^{T}}X \right)}^{-1}}$ 如果特征数量n较大则运算代价大，因为矩阵逆的计算时间复杂度为$O\left( {{n}^{3}} \right)$，通常来说当$n$小于10000 时还是可以接受的 |
| 适用于各种类型的模型       | 只适用于线性模型，不适合逻辑回归模型等其他模型                  |


## 多元线性回归 
> 均值归一化 Mean normalization(特征缩放)
> $ {\theta} $ 向量与${X}$ 向量代替原本的$ {\theta} $ 与$X$

## 逻辑回归 logistic regression （分类问题）

逻辑回归模型的假设是： $h_\theta \left( x \right)=g\left(\theta^{T}X \right)$
其中：
$X$ 代表特征向量
$g$ 代表逻辑函数（**logistic function**)是一个常用的逻辑函数为**S**形函数（**Sigmoid function**），公式为： $g\left( z \right)=\frac{1}{1+{{e}^{-z}}}$。

## 分类问题（一对多
- 转化为多个1对1的问题。（每次判断是不是其中的一类，结果作为置信度


#### 过拟合问题
- 调整参数权重 
> 1.在代价函数中添加正则项
- 减少变量
> 1. 相关性分析 KL（相关性系数矩阵
