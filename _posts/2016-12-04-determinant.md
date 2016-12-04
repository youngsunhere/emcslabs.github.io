---
layout: post
title: Determinant
description: "What determinant represents"
headline: "What determinant represents"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---
## Determinant

$A = \begin{bmatrix} a & b\\\c & d \\\
\end{bmatrix}$

A의 determinant는 아래와 같이 구한다.

$ \begin{vmatrix} a & b \\\ c & d \end{vmatrix}= ad - bc$
행렬 A의 determinant (=ad-bc)는 2차원 평면에서 2개의 열벡터로 만들어지는 평행사변형의 넓이와 동일하다. <br><br>

$B = \begin{bmatrix} a & b & c\\\d & e & f \\\g & h & i\\\
\end{bmatrix}$

B의 determinant는 아래와 같이 구한다. <br>
$\begin{vmatrix} a & b & c \\\ d & e & f \\\ g & h & i\end{vmatrix}= a\begin{vmatrix} e & f \\\ h & i\end{vmatrix}-b\begin{vmatrix}d&f\\\g&i\end{vmatrix}+c\begin{vmatrix}d&e\\\g&h\end{vmatrix} \\\= a(ei-fh)-b(di-fg)+c(dh-eg) \\\= aei+bfg+cdh-ceg-bdi-afh.$

행렬 B의 determinant는 3차원 공간에서 3개의 열벡터로 만들어지는 box의 부피이다.  <br><br>

- n-by-n 행렬의 determinant는 그 행렬의 열벡터로 만들어지는 n차원 box의 부피이다.
- n차원 box를 생성하기 위해서는 n개의 벡터가 필요하므로 determinant란 자연히 square matrix에서만 구할 수 있게 된다.
- determinant가 0이라는 것은 n-by-n의 열벡터가 linearly dependent하기 때문에 n차원 공간 내에서 '부피'를 형성하지 못한다는 뜻이다. 예를 들어, 3차원인 3개의 열벡터가 linearly dependent하여 2차원 평면밖에 구성하지 못할 때, 그 box의 부피는 0이다. 
- determinant가 0인 행렬을 singular matrix라고 부른다. 
- determinant가 음수라 함은 n개 벡터의 orientation의 순서가 reverse되었다는 뜻일 뿐 그 절대값은 여전히 n차원 box의 부피와 동일하다 <br>






<p align="right"> Yeonjung Hong <p>
