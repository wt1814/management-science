
<!-- TOC -->

- [1. 抽样分布](#1-抽样分布)
    - [1.1. 抽样的基本概念](#11-抽样的基本概念)
        - [1.1.1. 总体与样本](#111-总体与样本)
        - [1.1.2. 抽样](#112-抽样)
    - [1.2. 【样本统计量】及其【分布】](#12-样本统计量及其分布)
        - [1.2.1. 统计量和统计量分布的定义](#121-统计量和统计量分布的定义)
        - [1.2.2. 样本的【均值（统计量）】的分布（`【中心极限定理】`）](#122-样本的均值统计量的分布中心极限定理)
    - [1.3. 样本统计量的`三大常用分布`](#13-样本统计量的三大常用分布)
        - [1.3.1. χ2分布](#131-χ2分布)
            - [1.3.1.1. 定义](#1311-定义)
            - [1.3.1.2. 数字特征](#1312-数字特征)
            - [1.3.1.3. 分位数](#1313-分位数)
        - [1.3.2. t分布](#132-t分布)
            - [1.3.2.1. 定义](#1321-定义)
            - [1.3.2.2. 数字特征](#1322-数字特征)
        - [1.3.3. F分布](#133-f分布)
        - [1.3.4. 应用](#134-应用)
    - [1.4. `【正态总体】`的【统计量（样本均值、样本方差）】的【分布】](#14-正态总体的统计量样本均值样本方差的分布)
        - [1.4.1. 单个正态总体的情形](#141-单个正态总体的情形)
        - [1.4.2. 两个正态总体的差](#142-两个正态总体的差)

<!-- /TOC -->


<img src="http://182.92.69.8:8081/img/drawio/statistics/statistics-2-2.drawio.png" style="zoom:100%">  

-------
1. `中心极限定理`（`样本均值的抽样分布`）  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-176.png" style="zoom:60%">    


2. `三大常用分布`
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-139.png" style="zoom:60%">     

3. `【正态总体】`的【统计量（样本均值、样本方差）】的【分布】  
&emsp; 定理一：（服从正态分布）样本服从正态，【`均值`服从`正态分布`】，【均值的变形服从标准正态】；  
&emsp; 定理二：（服从卡方分布）样本服从正态，【`方差`的变形服从`卡方分布`】；  
&emsp; 定理三：（服从t分布）样本服从正态，【`均值和方差`服从`t分布`】。    
&emsp; ~~定理四：两个正态总体的情形~~
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-140.png" style="zoom:60%">    


# 1. 抽样分布  
## 1.1. 抽样的基本概念
### 1.1.1. 总体与样本  
1. 总体：  
&emsp; 总体是研究对象某一方面的数量指标，其分布函数和数字特征分别称为总体分布函数和总体数字特征。总体分类，有限总体与无限总体。   
2. 样本：  
&emsp; 按照某种方式从总体中抽出的部分个体指标，称为样本，样本中的个体数目称为样本容量。  

### 1.1.2. 抽样  
1. 抽样分布：  
&emsp; 抽样分布是指根据从总体中抽取的随机样本所得到的统计量的分布。  
&emsp; `随机变量和抽样分布`：<font color = "clime">随机变量作为抽样分布的基础；抽样分布是随机变量的分布；抽样分布用于推断总体参数</font>。  
2. 抽样方式：有放回与无放回。  
3. `抽样方法`：（2020年真题）`简单随机抽样、分层抽样、整群抽样、系统抽样`  
    1. `简单随机抽样`  
    &emsp; 又称`完全随机抽样`，是`在无限总体中进行的无放回独立抽样`或`在有限总体中进行的有放回随机抽样`。这样得到的样本称为简单随机样本。这种抽样方法在理论上最易处理，但实施时较难。简单随机抽样通常用样本平均数来估计总体均值，即简单估计。  
    2. `分层抽样`   
    &emsp; 即将总体中的成员`按某种原则划分成若干个子总体`，每个子总体称为一个层，`在每层中独立进行简单随机抽样或其他抽样`。分层抽样的估计是先对各层进行，然后再综合成总体参数的估计。分层抽样适用于调查既需要对总体进行估计也需要对局部进行估计的情况。当层内成员差异较小，而层间成员差异较大时，分层抽样可以提高估计的精度。  
    3. `整群抽样`  
    &emsp; `即将总体中的成员分为若干群(或组)`，`从这些群(或组)中抽取部分群(或组)`，`【调查对象是被抽中的这些群(或组)中的所有成员】`。其优点是当被调查单位地理位置比较集中时，实施起来比较方便；缺点是由于调查单位集中在若干群或组中，而不能均匀地分布在总体的各部分。因此，其准确性较差，但可以通过适当地多抽样来得到弥补。  
    4. `系统抽样`   
    &emsp; 又称`等距抽样`，即将总体中的调查单位按某种次序排列，随机地选定初始单位，然后按相等的间距抽取其他样本单位。系统抽样的好处是总体各部分都能在一定程度上被包括到样本中，实施方便；缺点是当初始单位决定之后，样本只有一种组合，不再具有随机性，当次序排列具有周期性时，容易产生严重的偏差。因此，在进行等距抽样之前，对调查单位的排列次序必须进行细致研究，以避免这种情况的发生。  

<!-- 
答：几种简单的抽样方法如下：
(1)简单随机抽样，又称完全随机抽样，是在无限总体中进行的无放回独立抽样或在有限总体中进 行的有放回随机抽样。这样得到的样本称为简单随机样本。这种抽样方法在理论上最易处理，但实施时较 难。简单随机抽样通常用样本平均数来估计总体均值，即简单估计。
(2)分层抽样，即将总体中的成员按某种原则划分成若干个子总体，每个子总体称为一个层，在每层中独立进行简单随机抽样或其他抽样。分层抽样的估计是先对各层进行，然后再综合成总体参数的估计。 分层抽样适用于调查既需要对总体进行估计也需要对局部进行估计的情况。当层内成员差异较小，而层间  成员差异较大时，分层抽样可以提高估计的精度。
(3)整群抽样，即将总体中的成员分为若干群(或组),从这些群(或组)中抽取部分群(或组),  调查对象是被抽中的这些群(或组)中的所有成员。其优点是当被调查单位地理位置比较集中时，实施起 来比较方便；缺点是由于调查单位集中在若干群或组中，而不能均匀地分布在总体的各部分。因此，其准确性较差，但可以通过适当地多抽样来得到弥补。
(4)系统抽样，又称等距抽样，即将总体中的调查单位按某种次序排列，随机地选定初始单位，然后按相等的间距抽取其他样本单位。系统抽样的好处是总体各部分都能在一定程度上被包括到样本中，实 施方便；缺点是当初始单位决定之后，样本只有一种组合，不再具有随机性，当次序排列具有周期性时， 容易产生严重的偏差。因此，在进行等距抽样之前，对调查单位的排列次序必须进行细致研究，以避免这 种情况的发生。
-->

## 1.2. 【样本统计量】及其【分布】  

### 1.2.1. 统计量和统计量分布的定义  
1. 统计量：  
&emsp; 由样本值去推断总体情况，需要对样本值进行“加工”，这就要构造一些样本的函数，它把样本中所含的（某一方面）信息集中起来。  
&emsp; 统计量的定义：样本的任意`不含有总体分布未知参数`的函数。  

2. `常见的样本统计量`：  
&emsp; 包括样本的均值、样本的方差、样本的比例等。  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-16.png" style="zoom:80%">      

3. 样本的统计量的分布  
&emsp; `样本统计量的分布`是指在给定总体下，从这个总体中获取多个样本并`计算样本统计量`时，所得到的`样本统计量`的`分布情况`。  
&emsp; 【`样本统计量的分布`通常会随着样本量的增大而趋近于`正态分布`，这是由于`中心极限定理`的影响。】  

### 1.2.2. 样本的【均值（统计量）】的分布（`【中心极限定理】`） 
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-127.png" style="zoom:30%">    
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-128.png" style="zoom:30%">    
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-138.png" style="zoom:30%">    


## 1.3. 样本统计量的`三大常用分布`    
<!-- 
https://www.jianshu.com/p/e9ab4519856b
-->

### 1.3.1. χ2分布  

#### 1.3.1.1. 定义  
<!-- 
设 X1,X2,......Xn相互独立, 都``服从标准正态分布N(0,1)``, 则称随机变量χ2=X1²+X2²+......+Xn²所服从的分布为自由度为n的χ2分布.   
-->

1. 定义：  
&emsp; 若n个相互独立的随机变量ξ₁，ξ₂，...,ξn均服从`标准正态分布`（也称独立同分布于标准正态分布），则这`n个服从标准正态分布的随机变量`的`平方和`构成一新的随机变量（χ2=X1²+X2²+......+Xn²），其分布规律称为卡方分布。  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-17.png" style="zoom:20%">      
 
2. 自由度：  
&emsp; 所包含的独立变量的个数 （eg:χ2=X1²+X2²，自由度为2）  

3. 图和式子如下：  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-96.png" style="zoom:50%">      
&emsp; 从分布图可以看出：图像分布在第一象限内，卡方值都是正值，呈右偏态，随着参数n的增大，分布趋近于正态分布；随着自由度n的增大，向正无穷方向延伸（这是因为均值n越来越大），分布曲线也越来越低（因为方差2n越来越大）。  


#### 1.3.1.2. 数字特征  
1. χ2分布的期望和方差：  
&emsp; `E(χ2)＝n，方差D(χ2)＝2n`。  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-98.png" style="zoom:50%">      
2. χ2分布的可加性：  
&emsp; 若χ12～χ2（n1），χ22～χ2（n2），且相互独立，则χ12＋χ22～χ2（n1＋n2）。  


#### 1.3.1.3. 分位数  
&emsp; <img src="http://182.92.69.8:8081/img/stats/stats-18.png" style="zoom:50%">      


### 1.3.2. t分布  
#### 1.3.2.1. 定义  
1. 定义：  
    &emsp; <img src="http://182.92.69.8:8081/img/stats/stats-20.png" style="zoom:30%">      
    &emsp; <img src="http://182.92.69.8:8081/img/stats/stats-21.png" style="zoom:30%">      

2. 图和式子如下：  
    &emsp; <img src="http://182.92.69.8:8081/img/stats/stats-97.png" style="zoom:50%">      
    1. 图像整体以0为中心，左右对称的单峰分布；  
    2. t分布是一簇曲线，可发现其形态变化与n（即其自由度）大小有关。自由度n越小，t分布曲线越低平；自由度n越大，t分布曲线越接近标准正态分布曲线，当自由度无限大时，t分布就成了正态分布。   

#### 1.3.2.2. 数字特征  
&emsp; 期望E(T)=0； 方差D(T)=n/(n-2)，n>2  

### 1.3.3. F分布
<img src="http://182.92.69.8:8081/img/stats/stats-22.png" style="zoom:30%">      
<img src="http://182.92.69.8:8081/img/stats/stats-23.png" style="zoom:30%">      


### 1.3.4. 应用  
&emsp; 卡方分布常用于检验统计量的分布，例如检验方差的假设。  
&emsp; t分布适用于样本均值的抽样分布。  


## 1.4. `【正态总体】`的【统计量（样本均值、样本方差）】的【分布】
<!-- 
https://blog.csdn.net/SpiritedAway1106/article/details/108608994
https://blog.csdn.net/universe_1207/article/details/106118591
https://max.book118.com/html/2021/1020/8040021075004022.shtm

https://www.renrendoc.com/paper/203145680.html
-->

### 1.4.1. 单个正态总体的情形
1. 定理一：线性组合还服从正态分布  
<img src="http://182.92.69.8:8081/img/stats/stats-57.png" style="zoom:50%">    

2. 推论一：服从正态分布  
<img src="http://182.92.69.8:8081/img/stats/stats-58.png" style="zoom:50%">    

3. 定理二：服从卡方分布  
<img src="http://182.92.69.8:8081/img/stats/stats-55.png" style="zoom:50%">    

4. 定理三：服从t分布    
<img src="http://182.92.69.8:8081/img/stats/stats-56.png" style="zoom:50%">    


### 1.4.2. 两个正态总体的差
<img src="http://182.92.69.8:8081/img/stats/stats-59.png" style="zoom:50%">    
