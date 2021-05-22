---
layout: post
title: 线性空间(一)
date: 2021-01-18 15:00
category: Math
author: Bao
tags: [Math]
summary: 映射,线性空间与n维向量空间的定义
---

## 线性空间的定义

若对应法则f满足

 $$
 A\rightarrow B,其中每个a\in A对应唯一的b\in B
 $$

则称f是A到B的一个**映射**,b是a在 f下的**像**,记作f(a).称a是b在f下的*一个***原像**.

A称为**定义域(Domain)**,B称为**陪域**(Codomain).$f(A):= \{f(a)|a\in A\}$称为**值域**.

若f(A) = B,则f称为一个**满射**.
如果A中不同元素在f下的像不同,称f为**单射**.
如果f既是单射又是满射,则f称为一个**双射**(一一对应).

---

**定义** 笛卡尔积
$$
 S \times M :=\{(a,b)|a \in S,b \in M\} 
$$

称为S与M的**笛卡尔积**.

---

**定义1**

非空集合S上的一个**代数运算**是指$S\times S$到S的一个映射.

> 注意极限不是代数运算

---

**定义2**

设V是一个非空集合,K是一个数域.

如果V上有一个运算,称为加法,即

$$(\alpha ,\beta ) \rightarrowtail \alpha+\beta$$

K和V之间有一个运算,称为**数量乘法**.即 
$$
K \times V \rightarrow V:(k,\alpha) \rightarrowtail k\alpha
$$

且满足8条运算性质(不再赘述)

V就称为数域K上的一个**线性空间**.


## 线性空间的例子:n维向量空间

令
$$
 K ^{n} = \{(a_1,a_2,...a_n)|a_i \in K,i = 1,2,...,n \} 
$$

 规定
 $$
  (a_1,a_2,...a_n)=(b _1,b _2,...,b _n)\\
  \stackrel{\triangle}{\iff} \\
  a_i = b_i,i=1,2,...,n.
 $$

 规定

$$
\begin{aligned}
    数量乘法\ &k(a_1,a_2,,...,a_n)=(k a_1,k a_2 ,...,k a_n)\\
 加法\ &(a_1,a_2,...a_n)+(b _1,b _2,...,b _n)=(a_1+b _1,a_2+b _2,...,a_n+b _n)
\end{aligned}
$$ 

并满足8条运算性质

|加法|数乘
|---|---
|交换律|单位元素
|结合律|交换律
|零元素|左分配律
|负元素|右分配率

则 $K^n是一个K上的n维向量空间.$它是数域K上的一个线性空间.




## 其他可推出的性质

设V是数域K上的一个线性空间.

### (1)V的零元唯一

设 $O_1,O_2$都是V的零元,则
$$
     O_1 = O_1+\stackrel{零元}{O_2}  =O_2+\stackrel{零元}{O_1}= O_2 
$$

### (2)每个$\alpha \in V$的负元唯一

设$\beta_1,\beta_2$都是 $\alpha$的负元,则

$$
  \beta _1 + \alpha +\beta _2=\beta _1+(\alpha + \beta _2)=(\beta_1+\alpha )+\beta _2 = \beta _1 = \beta _2
$$

### (3) $0\alpha = \stackrel{零元}{ \vec{0}}$
$$
 0\alpha = (0+0)\alpha=0 \alpha + 0\alpha 
$$

两边加$0\alpha$的负元,得
$$
 0 = 0 \alpha  
$$

### (4)$k\vec{0}= \vec{0}$
>证明思路:零元是加法的性质,k0是数量乘法,要利用他们的"桥梁"性质8
$$
 k0=k(0+0)=k0+k0
$$

两边加k0的负元

$$
  0 = k\vec{0}
$$

### (5)$k\alpha = 0$则k = 0或者$\alpha = 0$

假设k = 0,则

$$
 \alpha = 1\alpha = kk ^{-1} \alpha =k (k\alpha) = k\mathbf0 \xlongequal{由(4)} \mathbf{0}
$$

### (6) $(-1)\alpha = -\alpha$
$$
(-1)\alpha + \alpha =(-1)\alpha + 1 \alpha =(-1+1)\alpha  = 0 \alpha \xlongequal{由(3)}\mathbf0
$$

## 线性子空间

定义 设V是数域K上的一个线性空间,U是V的一个非空子集,如果U对于V的加法和数量乘法也成为数域K上的一个线性空间,那么称U是V的一个线性子空间.