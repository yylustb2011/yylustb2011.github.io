---
title: 凸优化数学公式测试
date: 2026-10-26
math: true
---

本文介绍正定矩阵、二次函数梯度与 Hessian 矩阵的基本性质，并通过 LaTeX 展示多行公式和矩阵表达式。

<!-- more -->

## 1. 行内公式

对于正定矩阵 $P \succ 0$，有 $x^\top P x > 0$。

## 2. 多行公式

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