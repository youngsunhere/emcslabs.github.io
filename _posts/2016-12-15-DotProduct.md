---
layout: post
title: Dot Product
description: "Dot Product"
headline: "Dot Product"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Dot Product

- dot product는 차원이 같은 두 n차원 벡터 x, y를 element-wise 곱하여 더한 결과의 상수값이다.
- 이는  x<sup>T</sup>y와도 같다. 
	- x<sup>T</sup>란?
		- 1개의 n차원 벡터를 n개의 1차원 상수의 나열로 바꾼 것.
		- n차원에서 1차원으로의 transformation matrix.
	- x<sup>T</sup>y란?
		1. x<sup>T</sup>는 y를 x에 **projection**시킨다. <br>
				이 때문에,<br>
				- x와 y가 &ang;90: dot product = 0<br>
				- x와 y의 방향이 비슷: dot product &uArr;<br>
				- x와 y의 방향이 다름: dot product &dArr; (&ang;90 넘으면 음수)
		2. x에 project된 y를 x길이만큼 **scale**한다. 

<br>

- dot product = inner product = "project then scale"


	
	
	
<p align="right"> Yeonjung Hong <p>
