# 模拟电子技术

# Chap 0

## 课程 [模拟电子技术(清华大学)](https://www.bilibili.com/video/BV1Vp411f71S)

## 课本 [模拟电子技术(上)](../TextBooks/%E6%A8%A1%E6%8B%9F%E7%94%B5%E5%AD%90%E6%8A%80%E6%9C%AF%E5%9F%BA%E7%A1%80%E4%B8%8A%EF%BC%89.pdf)&emsp;[模拟电子技术基础(下)](../TextBooks/%E6%A8%A1%E6%8B%9F%E7%94%B5%E5%AD%90%E6%8A%80%E6%9C%AF%E5%9F%BA%E7%A1%80(%E4%B8%8B).pdf)

# Chap 1什么是半导体

## Chap 1.1.1 本征半导体

&emsp;导体和绝缘体之间的元素就叫半导体, 材料的导电性能主要由自由电子决定.
绝缘体一般是高价元素,或者高分子物质。
本征半导体是纯净的，晶体结构的半导体
![avatar](./images/benzhengbdt.png)
<font size = 2><center>本征半导体的结构</center></font>
&emsp;自由电子碰到空穴,二者就会同时消失,这称为复合,有一个自由电子就有一个空穴.
当价电子离开空穴和数量和自由电子复合的数量相等,我们将其成为动态平衡。
本征半导体中的两种载流子则为空穴和自由电子
半导体的导电性能和温度是有关的

## Chap1.1.2杂质半导体

### N(Neigative)型半导体|P(Positive)形半导体

&emsp;我们在本征半导体中掺入P元素,那么自由电子的数量比空穴就多,这和P的含量有关,这就使得半导体的导电性能可控
那么掺入B元素的时候,则恰好相反.
&emsp;注意空位和空穴的区别:空位是不带电的,而空穴是带正电的
![avatar](./images/npbdt.png)
<font size = 2><center>杂质半导体的结构</center></font>

### 多子和少子  

&emsp;多子指的是多数载流子,少子亦然
而且多子在温度下的浓度变化小于少子(使用比例)

## Chap1.1.3 PN结的形成

### 什么是PN结  

[PN结的wiki](https://zh.wikipedia.org/wiki/Pn%E7%BB%93)         
[Khan acadamy的视频](https://www.bilibili.com/video/BV13t411S7AB)   
![avatar](images/Form%20of%20PN%20Not.png)      
<font size = 2>PN结的结构</center></font>  
&emsp;这里的PN结不是将一个P形半导体和一个N形半导体贴在一起,PN结是一块完整的晶体,通过渗透工艺将其做成PN结.
中间的部分将会相互补充,湮灭。
&emsp;同时中间产生的电场会阻止这个效应继续进行,这样就形成了一个PN结,中间的部分我们一般叫耗尽层

### PN结的单向导电性能  

PN结的正向导通  
![avatar](./images/PN%E7%BB%93%E6%AD%A3%E5%90%91%E5%AF%BC%E9%80%9A.png)     
<b>&emsp;这时耗尽层的宽度变小,使得漫游作用减弱,使得PN结的导电性增强</b>
<b>&emsp;这里加保护电阻,以免烧坏</b>
![avtar](./images/PN%E7%BB%93%E5%8F%8D%E5%90%91%E5%AF%BC%E9%80%9A.png)  
<b>&emsp;这个时候则恰好相中间耗尽区变宽,使得PN结的导电性能减弱</b>  
这就解释了PN结为什么有单向导电性
[<font size = 4>Willam Shockery's Story</font>](https://zh.wikipedia.org/wiki/%E5%A8%81%E5%BB%89%C2%B7%E8%82%96%E5%85%8B%E5%88%A9)

## Chap1.1.4PN结的电容效应  

&emsp;势垒效应
指的是在反接电压的时候,耗尽区变宽,有一个电荷吞吐的过程,这个过程中PN结可以被等效为电容,这个电容被称为势垒电容,记为$C_{b}$
![avatar](./images/%E5%8A%BF%E5%9E%92%E6%95%88%E5%BA%94.png)
扩散效应
指的是在加正向电压的时候,耗尽区变窄,也有电荷吞吐的过程,也可以被记为电容,被称为扩散电容$C_{d}$
<font size = 3><center>所以 PN结是存在一定的结电容, 并且有以下的关系</center></font>

<font size = 3><center>$C_{j} = C_{b} + C_{d}$</center></font>      
这个电容的大小和PN结的面积以及外加电容的大小有关,所以PN结的单向导电性也是在一定电压范围内的

## Chap1.1.5几种常见的二极管 

![几种常见的二极管](./images/%E5%87%A0%E7%A7%8D%E5%B8%B8%E8%A7%81%E7%9A%84%E4%BA%8C%E6%9E%81%E7%AE%A1.png)      
&emsp;点接触型:这种PN结结电容小,允许流过的电容也小,最高工作频率高       
&emsp;面接触型:这种就是结电容大,电流大,最高工作频率较低     
&emsp;平面型:接触面积可大可小,那么就可以控制 

## 1.2.1半导体二极管的伏安特性和电流方程 
![avtar](./images/%E4%BA%8C%E6%9E%81%E7%AE%A1%E7%9A%84%E4%BC%8F%E5%AE%89%E7%89%B9%E6%80%A7%E6%9B%B2%E7%BA%BF.png)   
这个图像的函数如下:     
<font size = 5><center>$i= I_{S}(e^{qu/kt}-1 )$</center></font>
### 图解
&emsp;有以下几个量:  $U_{on}$&emsp;$U_{BR}$&emsp;$I_{S}$&emsp;   