---
layout: post
title: Orthogonalization
description: "Orthogonalization"
headline: "Orthogonalization"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Orthogonalization

어떤 벡터 공간 V을 span하면서 서로 직교하는 벡터들을 찾는 것을 orthogonalization이라고 한다. <br><br>
m-by-n 행렬 A가 orthogonalization을 거쳐 열벡터가 서로 직교하게 되면, 다음과 같은 이유로 유용하다.

1. 행렬의 형태를 단순화함으로써, 각종 연산이 손쉬워 진다.
   - A의 열벡터가 orthogonal하다면, A<sup>T</sup>A = diagonal matrix
   - A의 열벡터가 orthonormal하다면, A<sup>T</sup>A=I
   - A의 열벡터가 orthonormal하면서 m=n이면, A<sup>T</sup> = A<sup>-1</sup>
2. 특별한 기능을 수행하는 행렬을 만들어 낼 수 있다.
	- projection, rotation, reflection 모두 orthogonal matrix이다. 
		- Orthogonal matrix Q란?
			- orthonormal 벡터로 구성된 정사각 행렬
			- Q<sup>T</sup> = Q<sup>-1</sup>
			- Q는 1)입력 벡터의 길이를 유지하고 2) 입력 벡터들 간의 각도를 유지시킨다.<br>
			  => Q를 곱해도 벡터의 길이가 유지되므로, 컴퓨터 연산 과정에서 발생하는 반올림 문제(round off error)를 없앤다.	
	
	
<p align="right"> Yeonjung Hong <p>
