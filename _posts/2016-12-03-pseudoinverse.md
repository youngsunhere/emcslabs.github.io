---
layout: post
title: Pseudoinverse
description: "Pseudoinverse"
headline: "Pseudoinverse"
categories: Math
tags: 
  - Matrix
  - Pseudoinverse
  - Linear Algebra
comments: false
mathjax: true
featured: true
published: true
---

## Pseudoinverse

연립방정식을 풀 때 다음과 같이 inverse matrix을 이용하면 쉽게 그 해를 구할 수 있다.<br><br>
$2x  +  y =  4 \\\
x  +  y = 3$

$\begin{bmatrix}2 & 1 \\\ 1 & 1 \end{bmatrix} \begin{bmatrix}x \\\ y \end{bmatrix}=\begin{bmatrix} 4 \\\ 3 \end{bmatrix}$

$\begin{bmatrix}x \\\ y \end{bmatrix}=\begin{bmatrix}2 & 1 \\\ 1 & 1 \end{bmatrix}^{-1}\begin{bmatrix}4 \\\ 3 \end{bmatrix}=\begin{bmatrix}1 & -1 \\\ -1 & 2 \end{bmatrix}\begin{bmatrix}4 \\\ 3 \end{bmatrix}=\begin{bmatrix}1 \\\ 2 \end{bmatrix}$

하지만, square matrix가 아닌 경우의 inverse는 어떻게 구할까?

- m by n 직사각형 matrix에 자신의 transpose인 $A^{T}A$ 혹은  $AA^{T}$를 곱한 뒤 square matrix로 만든다. 이때, m 과 n 중 작은 수 (즉, rank) 의 square가 되도록 transpose 해주는 것이다.
-  그 square matrix의 inverse를 구하고,
- 다시, transpose를 곱해 원래의 직사각형 행렬로 돌아오면 된다.<br><br>

m > n: left inverse -> $(A^{T}A)^{-1}A^{T}$  
n > m: right inverse -> $A^{T}(AA^{T})^{-1}$  
left, right를 이렇게 구분하기 싫으면, SVD(singular vector decomposition)로 그냥 구하면 됨.

