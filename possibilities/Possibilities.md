# Possibilities

505

## 基本概念

1. 概率是频率的稳定
2. 注意次序问题 要想清楚

- 贝叶斯公式

  ==实质就是==

$$
P(A\mid B_i)和P(B_i\mid A)的关系
$$



## 随机变量的分布



1. 随机变量的概念

   概率分布函数

2. 伯努利分布   离散
   $$
   X\sim(n,p)
   $$

3. 泊松   *看作二项分布的极限*  离散
   $$
   P \lbrace X=k\rbrace =\frac{\lambda^k}{k!}e^{-\lambda}
   $$

   $$
   X \sim P(\lambda)
   $$

    ==前提是二项分布==

$$
\lim_{n \to \infty} np_n = \lambda > 0 
$$

$$
\lim_{n \to \infty} P\lbrace X_n=k \rbrace = \frac{\lambda^k}{k!}e^{-\lambda}
$$

​		其中
$$
\lambda = np
$$
​		泊松分布，重点是==等号==

​		表里面的是$$ F(X \geq x)  $$的值

​	4. 连续型随机变量
$$
F(x) = \int_{-\infty}^x f(u)du
$$
**对于连续型随机变量**
$$
P\lbrace x_1<X<x_2 \rbrace =P \lbrace x_1\leq X \leq x_2 \rbrace
$$
==概率为 0 不一定是不可能事件==

5. 几个分布

   均匀

   指数

   正态   记得区分正态分布和标准正态分布

6. 上侧分位数    

![image-20220506093149630](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220506093149630.png)

看教材 P56页的例子， 分位数就是一个指标

7. 条件概率密度

   因为不能保证分母不为0

   



## ==多维随机变量==

1.  P78

   第一次命中 i 次 第二次命中 j 次
   $$
   P = (1-p)^{(i-1)}.p.(1-p)^{(j-i-1)}.p  (1-p)^{(i-2)}.p
   $$
   
   
   
   第二次命中j次
   $$
   P = C_{(j-1)}^1(1-p)^{(i-1)}.p.(1-p)^{(j-i-1)}.p= (j-1).(1-p)^{(i-2)}.p^2
   $$
   

   
2. 注意！！

   $$ E^2(x)  和 E(x^2) $$
   $$
   E[ g (X) ] = \int_{- \infty}^{+\infty}g(x)f(x)dx
   $$
   





然后是重点：

3. 

- 联合概率密度  联合分布函数
- 边缘概率密度  边缘分布函数

![image-20220507122118463](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220507122118463.png)



4. 

![image-20220507203231325](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220507203231325.png)





## 随机变量的数字特征

1. 随机变量的数学期望

==对于Y=g( x )==

F（Y）的分布函数     y是一个过程量

和

E（Y）的数学期望     y是一个最终的结果量

2. 两变量**相互独立**

$$
E(XY)=E(X)E(Y)
$$

由此可以得出
$$
D(X\pm Y)=D(X)+D(Y)+2E\lbrace [X-E(x)][Y-E(Y)] \rbrace
$$
当 X和Y独立的时候  E可以直接进去

$$  E\lbrace [X-E(x)][Y-E(Y)] \rbrace = [E(x)-E(x)][E(y)-E(y)] =0 $$

3. 协方差

$$
Cov(X,Y)=E\lbrace [X-E(x)][Y-E(Y)] \rbrace
$$

![image-20220508160055736](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508160055736.png)

 但是对于 二位正太随机变量  **相互独立=不相关**

4. 矩

https://zhuanlan.zhihu.com/p/355838840

![image-20220508160757347](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508160757347.png)

> 统计学中，**概率**与物理中的**质量**相对应

https://zhuanlan.zhihu.com/p/357320540

这才是真正的数学, 真正的对宇宙的探索

之前完全对这些不了解

![image-20220508162821864](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508162821864.png)

## 大数定理 和 中心极限定理

![image-20220508163755413](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508163755413.png)

![image-20220508170915009](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508170915009.png)

中心极限定理

##  数理统计概念

![image-20220508171240219](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508171240219.png)

![image-20220508171340845](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508171340845.png)

![image-20220508172610338](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508172610338.png)

![image-20220508185552252](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508185552252.png)

![image-20220508185623832](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508185623832.png)
![image-20220508185638579](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508185638579.png)

## 参数估计

重点就是求参数

相当于 
$$
\overline X 已知
$$
![image-20220508190707356](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220508190707356.png)

点估计 

1. 矩估计 

   样本矩去估计总体矩

![image-20220510214734515](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510214734515.png)

![image-20220510214752600](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510214752600.png)

2. 极大似然估计

$$
\lbrace X1 = x1, X2=x2 ....\rbrace事件已发生
$$

![image-20220510215323117](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510215323117.png)

如何求==似然函数==  其实很简单 现在想明白了

见 书 P161页

![image-20220510221117974](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510221117974.png)

![image-20220510221150434](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510221150434.png)

3. 检验效果

**无偏性、有效性、相合性**

![image-20220510221604021](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510221604021.png)

![image-20220510222319780](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510222319780.png)

![image-20220510222332547](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510222332547.png)







![image-20220510223159219](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510223159219.png)
![image-20220510223210976](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510223210976.png)

所以，只有样本均值等于真值均值时，样本方差的均值才等于真值方差。由于样本的随机性，样本均值取值不一定，所以分母为n的估计量均值 <= 真值方差，为有偏估计![image-20220510223234516](https://raw.githubusercontent.com/RNCHEN/photo-326/master/blogImg/image-20220510223234516.png)

>  那为什么样本均值是总体均值的无偏估计

https://blog.csdn.net/qq_16587307/article/details/95787764

https://www.cnblogs.com/hithink/p/10968326.html