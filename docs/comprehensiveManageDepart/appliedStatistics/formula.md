
<!-- TOC -->

- [1. 公式](#1-公式)
    - [1.1. ★★★公式](#11-★★★公式)
    - [1.2. ★★★人民大学统计背题](#12-★★★人民大学统计背题)
    - [1.3. 区间估计一览表](#13-区间估计一览表)
    - [1.4. 假设校验一览表](#14-假设校验一览表)
    - [1.5. ★★★线性回归分析](#15-★★★线性回归分析)
    - [1.6. 滑动平均趋势剔除法](#16-滑动平均趋势剔除法)

<!-- /TOC -->



# 1. 公式 

## 1.1. ★★★公式  

```pdf
/docs/comprehensiveManageDepart/appliedStatistics/formula.pdf
```

## 1.2. ★★★人民大学统计背题

```pdf
/docs/comprehensiveManageDepart/appliedStatistics/statisReview.pdf
```


## 1.3. 区间估计一览表  
1. 单个正态总体（3）  
    1. 均值  
    &emsp; 大样本 ---> 总体方差已知  ---> 服从正态Z分布统计量（即推论一）  
    &emsp; 小样本 ---> 总体方差未知  ---> 服从T分布统计量（即定理三）  
    2. 方差  
    &emsp; 服从卡方分布统计量（即定理二）  

2. 双正态总体均值差（2）  
    &emsp; 两个总体方差已知 ---> 服从正态Z分布统计量  
    &emsp; 两个总体方差未知，但相等  ---> 服从T分布统计量  

3. 单比率（1）


4. 双比率（1）  


5. 一般总体均值  


https://blog.csdn.net/weixin_45800258/article/details/127984405?utm_medium=distribute.pc_relevant.none-task-blog-2~default~baidujs_baidulandingword~default-0-127984405-blog-112663540.235^v40^pc_relevant_anti_t3_base&spm=1001.2101.3001.4242.1&utm_relevant_index=3  
<img src="http://182.92.69.8:8081/img/stats/stats-118.png" style="zoom:100%">    </br>  


<img src="http://182.92.69.8:8081/img/stats/stats-104.png" style="zoom:100%">    </br>  


## 1.4. 假设校验一览表

<img src="http://182.92.69.8:8081/img/stats/stats-119.png" style="zoom:100%">    </br>  

-------------

<img src="http://182.92.69.8:8081/img/stats/stats-105.png" style="zoom:100%">    </br>  
<img src="http://182.92.69.8:8081/img/stats/stats-106.png" style="zoom:100%">    </br>  

-------------

一个正态总体【均值】的假设检验  
<img src="http://182.92.69.8:8081/img/stats/stats-46.png" style="zoom:100%">    </br>  

一个正态总体【方差】的假设检验  
<img src="http://182.92.69.8:8081/img/stats/stats-47.png" style="zoom:100%">    </br>  

两个正态总体【均值差】的假设校验  
<img src="http://182.92.69.8:8081/img/stats/stats-49.png" style="zoom:50%">    </br>  

关于比率p的假设检验  
<img src="http://182.92.69.8:8081/img/stats/stats-48.png" style="zoom:50%">    </br>  


## 1.5. ★★★线性回归分析  
<img src="http://182.92.69.8:8081/img/stats/stats-99.png" style="zoom:100%">    </br>  
<img src="http://182.92.69.8:8081/img/stats/stats-120.png" style="zoom:100%">    </br>  
<img src="http://182.92.69.8:8081/img/stats/stats-121.png" style="zoom:100%">    </br>  
<img src="http://182.92.69.8:8081/img/stats/stats-102.png" style="zoom:100%">    </br>  


## 1.6. 滑动平均趋势剔除法  
&emsp; 视频讲解：https://www.bilibili.com/video/BV1X84y197qT/?vd_source=9a9cf49f6bf9bd6a6e6e556f641ae9cb  

&emsp; 滑动平均趋势剔除法，又称趋势剔除法，假定时间序列的乘法模型中各时点的不规则波动I相互独立。因此，在对数据进行间隔长度m=12(如果是月资料)或m=4(如果是季度资料)的滑动平均后，就能够消除季节波动和不规则波动的影响，从而得到滑动平均趋势值T×C。将原数列除以滑动平均趋势值T×C,得到的百分比称为滑动平均百分比，即    
<img src="http://182.92.69.8:8081/img/stats/stats-122.png" style="zoom:50%">    </br>  
&emsp; 然后对其进行同月(或同季)平均，以便消除不规则波动因素I的影响，从而得到季节变动S。最后，将其调整为以100为基准的季节指数。   
&emsp; 滑动平均趋势剔除法测定季节变动的``步骤``如下：   
&emsp; (1)对原数据进行12个月(如果数据是月资料)或4个季度(如果数据是季度资料)的滑动平均，求出`滑动平均趋势值`；   
&emsp; (2)将各实际值除以相应的趋势值，得到`滑动平均百分比`；  
&emsp; (3)将`滑动平均百分比【重新按月(或季)排列】`，求出同月(或同季)平均数；  
&emsp; (4)将同月(或同季)平均数`除以总平均数`，得到季节指数S。  


&emsp; ★★★<font color = "red">小结：1. 计算移动平均值 ---> 2. 计算滑动百分比 ---> 3. 重新排列 ---> 4. 再次计算平均值 ---> 5. 滑动百分比 计算总平均数 ---> 6. 计算季节指数</font>  
