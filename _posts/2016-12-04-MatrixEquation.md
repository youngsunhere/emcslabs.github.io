---
layout: post
title: Matrix equation
description: "Matrix equation"
headline: "Matrix equation"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: true
published: true
---

## MATRIX equation
$Ax = b$ (N.B. $x$: unknown params)

**연립방정식 (여러 개의 모델을 동시에 만족시키는 해 구하기)**

$2x + y = 4 \\\ x + y = 3$

$\begin{bmatrix}2 & 1 \\\ 1 & 1 \end{bmatrix} \begin{bmatrix}x \\\ y \end{bmatrix}=\begin{bmatrix} 4 \\\ 3 \end{bmatrix}$

**Linear Regression (알고 있는 데이터로부터 하나의 모르는 모델을 추정하기: e.g., ANN)**

모르는 모델을 $ax + b = y$ 라고 하면,  n개의 $x$와 $y$의 데이터가 있다면 다음의 matrix equation을 세울 수 있다.

$\begin{bmatrix} x_1 & 1 \\\ x_2 & 1 \\\ x_3 & 1 \\\ x_4 & 1 \\\ x_5 & 1 \\\ x_6 & 1 \\\ . & . \\\ . & . \\\ . & .  \\\  x_n & 1 \end{bmatrix} \begin{bmatrix}a \\\ b \end{bmatrix}=\begin{bmatrix} y_1 \\\ y_2 \\\ y_3 \\\ y_4 \\\ y_5 \\\ y_6 \\\ . \\\ . \\\ . \\\ y_n\end{bmatrix}$






<p align="right"> Hosung Nam <p>
