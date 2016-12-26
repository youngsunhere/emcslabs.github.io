---
layout: post
title: Projection
description: "Projection"
headline: "Projection"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Projection은 "그림자 만들기" 

- Projection이란, 벡터 v에 손전등을 비추어 특정 subspace에 v의 그림자가 생기도록 하는 것이다.
	- Projection에는 두 가지 종류가 있다.
		1. 손전등을 특정 subspace에 수직으로 비추는 orthogonal projection
		2. 손전등을 특정 subspace에 비스듬하게 비추는 nonorthogonal (=oblique) projection 	
   - 선형대수에서 Orthogonal projection의 비중이 더 크므로, 이하 내용은 orthogonal projection에 대한 것으로 한정하겠다. 
	

- projection의 쓰임
	1. 선형 방정식 Ax=b의 해 구하기
		- Ax=b라는 식은,주어진 데이터 행렬 A와 벡터 b의 인과관계를 벡터 x를 구함으로써 밝히고자 한다. 
		- 그러나 b가 A의 column space(=range(A)) 안에 없다면, Ax=b의 해를 구할 수 없다. <br>
		  (거의 모든 경우에 이러하다. 특히 변수 개수보다 식의 개수가 더 많은 m>n의 경우가 다반사이며 해를 구할 수 없는 대표적인 경우이다.)
		- 해결책은 실제 데이터와의 오류를 최소화하는 x를 찾는 것. 답은 projection에 있다.
		- 그러한 x를 찾는 방법은 b를 range(A)에 projection하는 것!
	2. 각종 decomposition의 핵심 도구
		- QR decomposition 
		- Singular Value Decomposition
		- Eignevalue Decomposition
<br>
- projector P
	- P = P<sup>T</sup> : symmetric matrix, column space=row space
	- P<sup>2</sup> = P : idempotent matrix, projection을 한 번 하든, 두 번 하든 결과는 똑같다. 
	- p = Px : 벡터 p는 벡터 x를 range(P)에 projection한 결과이다.
	- e = x-p : 벡터 e는 x와 x의 그림자 간의 에러이며, P의 nullspace에 속해 있다. 
	- p&perp;e이므로 range(P)&perp;null(P)

<br>

- projector P 구하는 법
  1. Ax=b의 근사해를 구하기 위하여, b를 range(A)에 projection한 것을 Ax<sub>new</sub>라고 하자. A&perp;(b-Ax<sub>new</sub>)이므로 <br>
     A<sup>T</sup>(b-Ax<sub>new</sub>)=0<br>
     A<sup>T</sup>Ax<sub>new</sub>=A<sup>T</sup>b
  2. x<sub>new</sub> = (A<sup>T</sup>A)<sup>-1</sup>A<sup>T</sup>b
  3. Ax<sub>new</sub> = A(A<sup>T</sup>A)<sup>-1</sup>A<sup>T</sup>b
  4. P = A(A<sup>T</sup>A)<sup>-1</sup>A<sup>T</sup>

- 벡터 b를 벡터 a 위에 project 하는 법
	- a와 b의 내적을 a의 길이 제곱으로 나눠준 만큼을 a에 scale한다.
	- b projected onto a = ${a^\mathrm{T}b \over a^\mathrm{T}a}a$
		- a<sup>T</sup>b: b를 a에 project하고 a길이만큼 scale
		- a<sup>T</sup>a: a길이만큼 unscale
	
	
	
<p align="right"> Yeonjung Hong <p>
