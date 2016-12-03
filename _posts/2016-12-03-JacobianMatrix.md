---
layout: post
title: Jacobian Matrix
description: "Jacobian Matrix"
headline: "Jacobian Matrix"
categories: Math
tags: 
  - Matrix
  - Jacobian
  - Linear Algebra
comments: false
mathjax: true
featured: true
published: true
---

## Jacobian Matrix

forward kinematics는 joint angle($θ_1, θ_2$)로부터 end-effector의 위치($x_1, x_2$)를 계산한다.

그렇다면 joint angle 속도로부터 end-effector의 속도를 어떻게 구할까?
$x$는 $θ$의 함수이고,  $θ$는 다시 시간 $t$의 함수이다. 
x의 속도로 부터 chain rule을 이용하여,  $x$의 속도와 $θ$ 속도의 관계를 나타내는 편미분 matrix $\frac{dx}{dθ}$를 Jacobian matrix 라 한다. (독립변수인 $θ$가 2개이상일 경우 편미분이라 함.)

$\frac{dx}{dt}=\frac{dx}{dθ}\frac{dθ}{dt}$

Jacobian matrix가 full rank (square matrix)가 아닌 경우나 singular ($det(J)==0$) 인 경우를 제외하고는 항상 $θ$를 계산할 수 있다. 


<p align="right"> Hosung Nam <p>
