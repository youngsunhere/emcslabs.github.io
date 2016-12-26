---
layout: post
title: QR factorization
description: "QR factorization"
headline: "QR factorization"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Reduced QR factorization (=decomposition)

열벡터가 linearly independent한 m-by-n 행렬 A를 Q와 R, 2개의 행렬로 분해하는 방법이다. <br>
Full QR factorization은 잘 사용하지 않기에 Reduced QR factorization기법 설명만 적어두었다.

1. Q
 - Q의 column space = A의 column space
 - Q의 열벡터 = orthonormal basis
 - m-by-n
2. R
 - upper triangular matrix
 - Q의 orthonormal basis의 linear combination을 통해 A로 되돌릴 수 있게끔 하는 계수들의 모음
 - 역행렬을 구할 수 있음
 - 대각선 값은 양수임
 - n-by-n
 
- QR factorization를 할 수 있는 방법
  1. Gram-Schmidt Orthogonalization (a.k.a triangular orthogonalization)
  2. Householder Triangularization (a.k.a orthogonal triangularization)

- QR factorization을 하는 이유
  - Ax=b의 해를 구하기 위해
  - eigenvalue를 구하기 위해 
	
	
	
<p align="right"> Yeonjung Hong <p>
