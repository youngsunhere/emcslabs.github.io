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
2차원 벡터 x를, basis A의 좌표계로 표현하면 [x]<sub>A</sub> = [1;0],<br>
basis B의 좌표계로 표현하면 [x]<sub>B</sub> = [2;1] 이다.<br>
이것은 V의 basis마다 unit에 대한 정의가 다르기 때문이다.<br><br>

3m를 cm로 환산하려면 3에 100을 곱하듯이,<br>
[X]<sub>A</sub>를 [X]<sub>B</sub>로 바꾸어 표현하려면, [X]<sub>A</sub>에 어떤 2-by-2 행렬 P를 곱하면 된다. <br><br>
이 때 P를 change of basis matrix라고도 부르며 P를 곱한다는 것은<br>
기존 basis의 좌표계를 다른 basis의 좌표계로 transform 한다는 뜻이다.<br>
같은 것을 다른 언어로 표현하는 것이다. <br><br><br>
그렇다면 A<sup>-1</sup>BAx의 의미는 무엇일까?<br>
A가 change of basis matrix, B는 모종의 transformation을 일으키는 matrix라고 보면 된다.<br>
1) Ax <- x를 A의 basis 좌표계로 표현. <br>
2) BAx <- [x]<sub>A</sub>에 rotation, reflection 과 같은 transformation을 함.
3) A<sup>-1</sup>BAx <- transformation 이후의 결과를 기존 basis 상태로 돌려 둠.<br>
<br>
역행렬 A<sup>-1</sup>의 역할이란 3)에서 밝혔듯 바뀌어진 basis를 되돌려 놓는 것이다. 

	
	
	
<p align="right"> Yeonjung Hong <p>
