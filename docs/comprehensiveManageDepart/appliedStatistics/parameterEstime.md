
<!-- TOC -->

- [1. 参数估计](#1-参数估计)
    - [1.1. 点估计和区间估计的区别](#11-点估计和区间估计的区别)
    - [1.2. 参数的点估计](#12-参数的点估计)
    - [1.3. 参数的区间估计](#13-参数的区间估计)

<!-- /TOC -->


# 1. 参数估计  
<!-- 
https://www.bilibili.com/video/BV1DK411Q7kE/?p=2&spm_id_from=pageDriver&vd_source=9a9cf49f6bf9bd6a6e6e556f641ae9cb

区间估计   Chapter8区间估计   https://zhuanlan.zhihu.com/p/66269685
-->
&emsp; 参数估计是通过使用样本数据来推断总体参数的过程。在统计学中，`总体`是指整个群体，而`样本`是从总体中选择的一部分观察结果。`参数`是`总体的特征数值`，例如`总体均值、总体方差`等。`参数估计`的目标是根据样本数据推断总体参数的可能值范围。  

<!-- 

大纲
&emsp; (1)考试范围  
&emsp; 参数点估计的计算方法，点估计的评价标准，双侧与单侧区间估计；关于一个正态总体参数的区间估计，关于总体比率的区间估计，关于两个正态总体均值差的区间估计，关于两个总体比率差的区间估计；样本容量的确定。  
&emsp; (2)考试要求  
&emsp; 了解估计量的概念，掌握参数点估计的计算方法：矩估计法；掌握 点估计量的评价标准：无偏性、有效性和一致性，并能够应用这些评价标准对统计量进行评价。
掌握单、双侧参数区间估计的差别，能根据实际问题选择应用双侧或单侧区间估计。  
&emsp; 掌握以下关于总体参数的区间估计：在已知或未知总体方差的条件下对总体均值进行区间估计；在已知或未知总体方差的条件下对两个总体均值差进行区间估计；在未知总体均值条件下对总体方差进行区间估计；在大样本情况下对总体比率进行区间估计；在大样本情况下对两个总体比率的差进行区间估计。能够应用置信水平和区间长度的关系确定样本容量。  
-->

## 1.1. 点估计和区间估计的区别    
1. 含义  
    1. 点估计是用样本统计量来估计总体参数，因为样本统计量为数轴上某一点值，估计的结果也以一个点的数值表示，所以称为点估计。  
    2. 区间估计是在点估计的基础上，给出总体参数估计的一个区间范围，该区间通常由样本统计量加减估计误差得到。  
    &emsp; 点估计量是用于估计总体参数的样本统计量。但不可能期望点估计量能给出总体参数的精确值，所以经常在点估计上加减一个被称为边际误差的值来计算区间估计。  
    &emsp; `区间估计的一般形式为`：`点估计±边际误差`。  
    &emsp; 区间估计的目的在于，提供基于样本得出的点估计值与总体参数值的接近程度方面的信息。  

2. 两者主要区别  
    1. 值不同  
    &emsp; 点估计的精确程度用置信区间表示。由样本数据估计总体分布所含未知参数的真值，所得到的值，称为估计值。  
    &emsp; 区间估计，是参数估计的一种形式。通过从总体中抽取的样本，根据一定的正确度与精确度的要求，构造出适当的区间，以作为总体的分布参数(或参数的函数)的真值所在范围的估计。  
    2. `是否考虑抽样误差`  
    &emsp; `点估计`是在抽样推断中`不考虑抽样误差`，直接以抽样指标代替全体指标的一种推断方法。因为个别样本的抽样指标不等于全体指标，所以，用抽样指标直接代替全体指标，不可避免的会有误差。  
    &emsp; `区间估计`是抽样推断中根据`抽样指标和抽样误差`去估计全体指标的可能范围的一种推断方法。在从抽样指标推断全体指标时，用一定概率保证误差不超出某一给定范围。  
    3. 常用方法不同   
    &emsp; 点估计的常用方法有矩估计法、顺序统计量法、最大似然法、最小二乘法等。   
    &emsp; 区间估计求置信区间的方法，最常用的求置信区间及置信上、下限的方法有利用已知的抽样分布（见统计量）、利用区间估计与假设检验的联系、利用大样本理论（见大样本统计）。   
3. 点估计、区间估计与校验   
&emsp; 区间估计是介于估计和检验之间的内容，且区间估计与检验紧密相连，因此有的也把区间估计看作是检验的一种。    


## 1.2. 参数的点估计  
&emsp; [3.1.参数的点估计](/docs/comprehensiveManageDepart/appliedStatistics/pointEstimation.md)   


## 1.3. 参数的区间估计 
&emsp; [3.2.参数的区间估计](/docs/comprehensiveManageDepart/appliedStatistics/intervalEstimation.md)   
