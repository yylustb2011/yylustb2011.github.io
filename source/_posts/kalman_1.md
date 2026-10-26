---
title: Kalman 滤波 - 1. 预备知识
date: 2026-10-26
math: true
---

本文介绍正定矩阵、二次函数梯度与 Hessian 矩阵的基本性质，并通过 LaTeX 展示多行公式和矩阵表达式。

<!-- more -->

# 1. 一维高斯分布
## 1.1 一维概率密度、均值与方差

## 1.1 一维概率密度、均值与方差

设 $X\sim\mathcal{N}(\mu,\sigma^2)$，其中 $\sigma>0$。它的概率密度函数为
$$
\begin{aligned}
p_X(x)
&=\frac{1}{\sqrt{2\pi\sigma^2}}
\cdot
\exp\left(-\frac{(x-\mu)^2}{2\sigma^2}\right)
\end{aligned}
$$
均值 $\mu=\mathbb{E}[X]$ 决定密度曲线的中心；方差
$$
\sigma^2=\mathbb{E}\left[(X-\mu)^2\right]
$$
衡量围绕中心的波动程度。



## 1.2 多行公式

$$
\begin{aligned}
f(x) &= \frac{1}{2}x^\top P x + q^\top x,\\
\nabla f(x) &= Px+q,\\
\nabla^2 f(x) &= P.
\end{aligned}
$$

## 3. 矩阵公式

$$
P =
\begin{bmatrix}
p_{11} & p_{12}\\
p_{21} & p_{22}
\end{bmatrix}.
$$

## 4. 定理

**定理：** 若 $P=P^\top\succ 0$，则二次函数

$$
f(x)=\frac{1}{2}x^\top Px+q^\top x
$$

存在唯一的全局最优解。