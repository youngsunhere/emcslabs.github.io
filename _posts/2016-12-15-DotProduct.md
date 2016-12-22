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

- dot product는 차원이 같은 두 n차원 벡터 x, y를 element-wise 곱하여 더한 결과이다(상수값).
- 이는  x<sup>T</sup>y와도 같다. 
	- x<sup>T</sup>란?
		- 1개의 n차원 벡터 -->  n개의 1차원 벡터의 나열.
		- n차원 인풋을 1차원 아웃풋으로 transform하는 matrix.
	- x<sup>T</sup>y란?
		1. x<sup>T</sup>는 y를 x에 **projection**시킨다. <br>
				이 때문에,<br>
				- x와 y가 &ang;90: dot product = 0<br>
				- x와 y의 방향이 비슷: dot product &uArr;<br>
				- x와 y의 방향이 다름: dot product &dArr; (&ang;90 넘으면 음수)
		2. x에 project된 y를 x길이만큼 **scale**한다. 
	- x<sup>T</sup>x
		- x를 x에 project한 뒤, x만큼 scale => **x 길이의 제곱**
<br>

- dot product = inner product = "project then scale"
<br><br>
따라서, 두 벡터의 dot product는 **1)벡터 간의 각도 2)두 벡터의 길이 정보**를 담고 있다. 	
	
	
<p align="right"> Yeonjung Hong <p>
