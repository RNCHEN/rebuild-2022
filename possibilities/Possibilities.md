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

   



## 多维随机变量

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
   





















