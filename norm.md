## 范数概述

&emsp;&emsp;`范数（Norm）`是在广义长度定义下，对函数、向量和矩阵的一种度量定义。在泛函分析中，范数是一个函数，是为向量空间内所有向量赋予的非零的正长度或大小。与之相关的还有`半范数（seminorm）`的概念，可以为非零的向量赋予零长度。一般来说，拥有范数的向量空间称之为赋向量空间，拥有半范数的向量法空间称之为赋半范向量空间。

## 定义

&emsp;&emsp;假设$V$是域$F$上的向量空间，$V$的`半范数`是一个函数$p: V\to  \mathbb R；x \mapsto p(x)$，满足：
>   $\forall a \in F，\forall \mu,v \in V$有:
> 
>   $p(v) \geq 0$（具有半正定义）
> 
>  $p(av)=|a|p(v)$（具有绝对一次齐次性）
>
>  $p(\mu+v) \leq p(\mu)+p(v)$（满足三角不等式，或次可加性）

&emsp;&emsp;范数是特殊的半范数，是满足如下性质的半范数：
> $p(v)=0$，当且仅当$v$是零向量时（正定性）

&emsp;&emsp;约定范数$p(x)=\|x\|$

---

## 向量范数

&emsp;&emsp;向量$X=(x_1,x_2,\dots,x_n)^T$的$p$范数定义为：
$$\| X \|_p=(\sum_{i=1}^{n}x_{i}^p)^{\frac{1}{p}}，p\in [1,+\infty]$$

&emsp;&emsp;常用的向量范数有1范数、2范数和无穷范数如下：
$$\|x\|_1=\sum_{i=1}^n|x_i|$$
$$\|x\|_2=(\sum_{i=1}^nx_i^2)^{\frac{1}{2}}$$
$$\|x\|_{\infty}=\lim_{p \to \infty}(\sum_{i=1}^nx_i^p)^{\frac{1}{p}}=max_{1 \leq \leq n}\{|x_i|\}$$

---
## 矩阵范数
&emsp;&emsp;基于向量范数可进一步定义矩阵范数，设$A \in \mathbb R^{n\times n}$，记方阵$A$的范数为$\|A\|$，则：
$$\| A  \| = sup_{x \in \mathbb R,x \neq 0}$$

&emsp;&emsp;对应与三种向量范数，相对应的三种矩阵范数形式如下：

$$\|A\|_1=max_{1 \leq j \leq n}\sum_{i=1}^{n}|a_{ij}|$$
$$\|A\|_2=(\rho(AA^T))^{\frac{1}{2}}$$

&emsp;&emsp;$\rho(A)=max_{i}|\lambda_i|$成矩阵$A$的谱半径，其中$\lambda_i$为矩阵$A$的特征值。

$$\|A\|_1=max_{1 \leq i \leq n}\sum_{j=1}^{n}|a_{ij}|$$

---