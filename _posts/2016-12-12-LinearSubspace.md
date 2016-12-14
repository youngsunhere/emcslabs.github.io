---
layout: post
title: Linear Subspace
description: "What is linear subspace?"
headline: "linear subspace"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Linear Subspace

- N차원 벡터 공간 V
	- linearly independent 한 N차원 벡터 N개의 linear combinations(=덧셈 + 상수배).<br><br>
- V의 linear subspace
	- N차원 벡터공간의 원소 벡터 M개의 linear combinations.
	- N차원 이하의 공간을 나타내는 V의 부분집합.
	- V가 3차원 벡터 공간일 때, V의 subspace가 될 수 있는 것은 아래와 같다. 
		- V
		- 원점([0;0;0])을 지나는 어떠한 평면
			- 예시: Span{[1;0;0], [0;1;0]}
		- 원점([0;0;0])을 지나는 어떠한 선분
			- 예시: Span{[1;0;0]}
		- 원점([0;0;0])
	- Q: [1;1]는 3차원 벡터 공간에서 평면을 이루는 subspace의 원소일 수 있을까?  
		- 아니다. 2차원 공간 내에 있긴 하지만 형태상으로는 3차원이어야 한다. 따라서 예를 들어 [1;1;0]은 가능하다. <br><br>
- Why linear?
	- linear transformation, linear subspace, linear combination... 모든 말 앞에 linear가 붙는다. 
	- 공간의 linearity는 그 공간을 구성하는 벡터들의 linearity에 의해 결정된다. 
	- linear vector의 집합은 linear subspace 이고, nonlinear vector의 집합은 nonlinear subspace이다.
	- nonlinear한 것의 대표적인 것은 곡선이나 곡면이다. 
	- linearity를 유지시키는 조건
		- 벡터 공간 안에서 덧셈과 상수배만 가능하다. (곱셈을 하는 순간 휘어진다.) <br/> 이 덕분에, 
			- 어느 공간에서나 단위벡터를 기준으로 눈금을 그렸을 때, <br/> 동일한 원점을 공유하고<br/>눈금선의 간격이 일정하고<br/>눈금선들이 서로 평행을 이룬다.


<p align="right"> Yeonjung Hong <p>
