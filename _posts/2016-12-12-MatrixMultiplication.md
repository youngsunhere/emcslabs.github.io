---
layout: post
title: Matrix Multiplication
description: "Matrix Multiplication"
headline: "Matrix Multiplication"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Matrix Multiplication

길이를 재는 단위에는 여러가지가 있으며, 모든 길이 표현은 특정 단위를 취한다.<br>
같은 물건을 100cm로 표현하기도 하고, 1m로 표현하기도 한다. <br><br>
마찬가지로,벡터 공간 V의 basis에는 여러가지가 있으며, 모든 벡터는 특정한 basis의 좌표계를 취한다. <br>
2차원 벡터 x를, basis A의 좌표계로 표현하면 다음과 같다. <br>
$[x]<sub>A</sub> = \begin{bmatrix} 1 & 0 \end{bmatrix}$<br>
basis B의 좌표계로 표현하면 다음과 같다. <br>
$[x]<sub>B</sub> = \begin{bmatrix} 2 & 1 \end{bmatrix}$<br>
이것은 V의 basis마다 unit에 대한 정의가 다르기 때문이다.<br><br>

3m를 cm로 환산하려면 3에 100을 곱하듯이,<br>
[X]<sub>A</sub>를 [X]<sub>B</sub>로 바꾸어 표현하려면, [X]<sub>A</sub>에 어떤 2-by-2 행렬 P를 곱하면 된다. <br><br>
행렬이 transformation function이라 함은,<br>
기존 basis의 좌표계를 다른 basis의 좌표계로 transform 한다는 뜻이다.<br>
같은 것을 다른 언어로 표현하는 것이다. 
	
	
	
<p align="right"> Yeonjung Hong <p>