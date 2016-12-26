---
layout: post
title: Inverse, Pseudoinverse, Transpose
description: "Inverse, Pseudoinverse, Transpose"
headline: "Inverse, Pseudoinverse, Transpose"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---


## m-by-n 행렬 A에 대한 A<sup>-1</sup>, A<sup>T</sup>, A<sup>+</sup> 정리

- A
	- A의 **row space에 있는 벡터**를 **column space에 있는 벡터**로 transform하는 함수

- A<sup>-1</sup>
	- A의 **column space에 있는 벡터**를 **row space에 있는 벡터**로 transform하는 함수. 
		- A가 full rank이고 정사각 행렬일 때(rank=m=n), A<sup>-1</sup> 존재함.
		- A<sup>-1</sup>가 존재한다.<br>
		  = A는 nonsingular다.<br>
		  = A의 nullspace에는 0벡터 뿐이다.
		  
- A<sup>T</sup>
	- A의 **column space에서 row space로 공간은 이동**시켜주지만 개별 벡터간 **일대일 역매핑은 못한다**. 
	- A가 남자 1호,2호,3호를 각각 여자 1호,2호,3호와 매칭시키는 함수라고 해보자. A<sup>-1</sup>는 A가 그은 사랑의 작대기를 유지시킨채 여자 셋을 남자 셋에게 매칭시켜준다면, A<sup>T</sup>는 여자 셋을 남자 셋과 매칭시켜주긴 하지만 기존의 작대기를 유지한다는 보장이 없다. 
- A<sup>+</sup>
	- A<sup>-1</sup>가 존재하지 않으면 pseudoinverse A<sup>+</sup>를 사용한다.
	- A<sup>+</sup>는 column space의 벡터들 중 row space에 대응 벡터가 있는 경우에 한하여 inversion을 수행한다.  
		- A<sup>+</sup>Ax=x는 row space에 있는 x에 대해 성립한다. 
		- A<sup>+</sup>Ax=x는 nullspace에 있는 x에 대해 성립하지 않는다. 
		- 0으로부터 nullspace의 모든 벡터를 복구하기는 불가능하기 때문이다. 


<p align="right"> Yeonjung Hong <p>
