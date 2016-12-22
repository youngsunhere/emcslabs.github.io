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

벡터 공간 V의 basis에는 여러가지가 있으며, <br>
그 중 대표적인 것은 서로 직교하면서 길이가 1인 벡터로 구성된 orthonormal basis이다.<br>
Cartesian 좌표계의 축도 일종의 basis로 보면 된다. <br><br>
동일 벡터 공간 V의 basis마다 unit의 정의가 다르기 때문에, 하나의 벡터를 basis마다 다르게 표현한다. <br>
예를 들어, x,y축을 갖는 2차원 공간의 basis A={[1;0],[0;1]}는 벡터 v를 [5;1]로 표현하지만, <br>
basis B={[2;1],[1;2]}는 벡터 v를 [3;-1]로 표현한다. <br><br>
이렇듯 어떤 벡터를 basis A에서 basis B로 바꾸어 표현하려면 change of basis matrix P<sub>B&larr;A</sub>를 곱하면 된다. <br>
사실상 모든 행렬은 basis를 바꾸는 기능을 하는 함수인데,<br>
그 결과 rotation, projection 등 유용한 기능을 수행하면 특별 취급받는 것이다. <br>
<br>

- A<sup>-1</sup>BAx의 의미<br>
A가 change of basis matrix, B는 모종의 transformation을 일으키는 matrix라고 보면 된다.<br>
1) Ax:  x를 A의 basis 좌표계로 표현. <br>
2) BAx:  [x]<sub>A</sub>에 원하는 transformation 수행. <br>
3) A<sup>-1</sup>BAx: transformation 이후의 결과를 기존 basis 상태로 돌려 둠.<br>
<br>
역행렬 A<sup>-1</sup>의 역할이란 3)에서 밝혔듯 바뀌어진 basis를 되돌려 놓는 것이다. 

	
	
	
<p align="right"> Yeonjung Hong <p>
