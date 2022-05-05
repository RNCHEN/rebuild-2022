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

2. 伯努利分布
   $$
   X\sim(n,p)
   $$

3. 泊松   *看作二项分布的极限*
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