---
layout: post
title: Column Space, Nullspace, Invertibility
description: "Column Space, Nullspace, Invertibility"
headline: "Column Space, Nullspace, Invertibility"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Column Space, Nullspace, Invertibility

m-by-n 행렬 A과 m차원 벡터 b가 있다. <br> 
여기에 n차원 미지수 벡터 x를 도입하면 Ax=b라는 방정식을 세울 수 있다. <br> 
Ax=b는 다음과 같이 읽을 수 있다. <br> 
"A는 **x**를 A의 **column space에 있는 b**로 transform한다."<br>
여기서 A의 column space란, A의 열벡터가 span하는 subspace이다.<br>
b는 A의 열벡터에 x의 원소를 각각 곱하여 더한 것으로서 열벡터의 linear combination이므로, A의 column space 안에 존재한다.<br><br>
함수로서의 A를 깊이 이해하기 위해서는 함수의 기본 성질을 이해해야 한다. <br>
함수는 하나 이상의 입력에 대하여 하나의 출력만 내놓는다. 즉 일대일 매핑, 다대일 매핑은 가능하지만 일대다 매핑은 불가능하다.<br>
역함수란 출력에서 입력으로의 역매핑을 하는데, 원래 함수가 다대일 매핑이면 역으로는 일대다 매핑이므로 역함수 성립이 불가능하다. <br>
따라서 일대일 매핑인 함수만 역함수를 갖는다.<br><br>
행렬 A 또한 일대일 매핑을 할 때만 역행렬을 갖는다.  <br>
A가 일대일 매핑을 한다는 뜻은, Ax=b에서 A가 어떤 두 입력 벡터 x도 A의 column space에 있는 동일한 벡터 b로 transform하지 않는다는 것이다.<br>
<br>
반면, A가 0벡터 뿐 아니라 0이 아닌 입력 벡터 x를 column space에 있는 0벡터로 transform한다면, A는 다대일 매핑을 하고 있으므로 역행렬이 존재하지 않는다.<br>
다른 말로 표현하면, Ax=0에 0이 아닌 해가 존재할 때 A는 역행렬이 없다. <br>
이 때 Ax=0을 만족시키는 x는 A의 nullspace를 구성한다. 

# 정리

m-by-n 행렬 A에 대하여, <br>

- The column space of A
   - A의 열벡터가 span하는 공간이다.
   - column space = range
	
- The nullspace of A
   - Ax=0를 만족하는 모든 n차원 벡터 x의 집합이다. (이 때 우항의 0은 상수가 아니라 m차원 0벡터)

방정식 Ax=b에 대하여, <br>

- 행렬 A는 입력 벡터 x를 linear combination을 통해 A의 column space에 있는 벡터 b로 transform한다.
- A의 역행렬이 존재한다. <br>
  = A가 일대일 매핑을 한다.<br>
  = Ax=b의 모든 m차원 벡터 b에 대하여 유일한 해 x가 존재한다.<br>
- A의 역행렬이 존재하지 않는다. <br>
  = Ax=0의 해가 0벡터 말고도 존재한다.<br>
  = A가 다대일 매핑을 한다. <br>
  = A의 nullspace에 0벡터가 아닌 다른 벡터도 존재한다. 


<p align="right"> Yeonjung Hong <p>
