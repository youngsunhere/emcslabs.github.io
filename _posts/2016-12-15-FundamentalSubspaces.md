---
layout: post
title: Fundamental Subspaces
description: "fundamental subspaces"
headline: "Fundamental Subspaces"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Fundamental Subspaces

m-by-n 행렬 A은 n차원 공간 R<sup>n</sup>에서의 좌표값을 m차원 공간 R<sup>m</sup>에서의 좌표값으로 transform한다.<br>
R<sup>n</sup>과 R<sup>m</sup>에는 무한한 subspace가 존재하는데, <br>
그 중 4가지 fundamental subspaces를 알아야 한다.

- R<sup>m</sup>의 2가지 fundamental subspaces
	- The column space of A = C(A)
	- The left nullspace of A = N(A<sup>T</sup>)

- R<sup>n</sup>의 2가지 fundamental subspaces
	- The nullspace of A = N(A)
	- The row space of A = C(A<sup>T</sup>)
		


4가지 중 column space와 nullspace만 제대로 이해하면 나머지 두 subspace는 절로 이해된다. 

- The column space of A
	- A의 열벡터 n개가 span하는 공간이다.
	- A에 n차원 벡터 x를 곱한 결과는 A의 열벡터의 linear combination이므로 b 역시 A의 column space 안에 존재한다. 
	- column space = range
	- column space의 차원 <br>
	  = column space의 basis에 들어있는 벡터 수 <br>
	  = linearly independent한 열벡터 수 <br>
	  = 행렬의 rank
	- Ax=b의 해가 존재한다 <br>
	  = b가 A의 column space에 들어있다. <br>
	  = m차원 좌표계로 표현한 b는 n차원 좌표계로도 표현할 수 있다. <br>
	  = A는 square matrix이고 역행렬이 존재한다.<br>
	  = A의 n개의 열벡터가 linearly independent하다.<br>
	  = A의 rank가 n이다. (<-full rank)<br>
	  = A의 column space=R<sup>m</sup><br>
	  = m=n	
 
<br>

- The nullspace of A
	- Ax=0를 만족하는 모든 n차원 벡터 x의 집합이다. (이 때 우항의 0은 상수가 아니라 m차원 0벡터)
	- Ax=0를 만족하는 벡터 x는 A의 행벡터들과의 inner product가 0이다. <br>
	  = A의 모든 행벡터들과 x는 cosine similarity가 0이다. <br>
	  = A의 모든 행벡터들과 x는 orthogonal하다. <br>
	  = A의 행벡터들이 span하는 row space와 x는 orthogonal하다. <br>
	  = A<sup>T</sup>의 열벡터들이 span하는 column space와 x는 orthogonal complement이다.<br>
	  = N(A)&perp;C(A<sup>T</sup>)
	- A의 열벡터가 linearly independent하다. <br>
	  = nullspace에는 0벡터 하나만 존재한다. <br>
	  = Ax=0의 해는 0벡터 외엔 없다. <br>
	  = A는 square matrix이고 역행렬이 존재한다. 
	- 통계적 관점에서, nullspace란 모든 샘플에서 구한 독립변수 값에 파라미터 x를 곱해주면 결과가 전부 0이 나오게끔 하는 파라미터 x의 집합이다. <br>
	  따라서 nullspace에 0이 아닌 벡터가 존재한다면 종속변수가 독립변수에 의해 설명되지 않는 면이 있다는 것을 의미한다. (noise가 없다고 가정했을 때) 
	
<br>

- N(A)&perp;C(A<sup>T</sup>)와 같은 이유로 C(A)&perp;N(A<sup>T</sup>)
<br>

- 모든 행렬은 row space에서 column space로의 transformation matrix다.

<p align="right"> Yeonjung Hong <p>
