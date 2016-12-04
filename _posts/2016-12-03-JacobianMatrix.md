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

forward kinematics는 joint angle($θ_1, θ_2$)로부터 end-effector의 위치($x_1, x_2$)를 계산하고,  joint angle 속도로부터 end-effector의 속도를 구하는 과정이다.

joint angle($θ_1, θ_2$)로부터 end-effector의 위치($x_1, x_2$)를 계산하는 과정은 쉽고 단순하므로 생략하고, joint angle 속도로부터 end-effector의 속도를 구하는 과정을 기술하면 다음과 같다. $x$는 $θ$의 함수이고,  $θ$는 다시 시간 $t$의 함수이다. x의 속도로 부터 chain rule을 이용하여,  $x$의 속도와 $θ$ 속도의 관계를 나타내는 편미분 matrix $\frac{dx}{dθ}$를 Jacobian matrix 라 한다. (독립변수인 $θ$가 2개이상일 경우 편미분이라 함.)

$\frac{dx}{dt}=\frac{dx}{dθ}\frac{dθ}{dt}=J\frac{dθ}{dt}$

$\dot{x}=J\dot{θ}$

$θ$에서 $x$,  $\dot{θ}$에서 $\dot{x}$의 계산이 forward kinematics이다. 하지만, 이 방향보단 반대의 방향, 즉 $x$에서 $θ$,  $\dot{x}$에서 $\dot{θ}$의 계산인 inverse kinematics가 현실에 더 필요하다. $θ$에서 $x$로의 직접적인 inverse kinematics는 도출이 힘들지만, $\dot{θ}$에서 $\dot{x}$의 forward kinematics는 $J$만 inverse 취하면 쉽게 그 inverse kinematics를 구할 수 있다.

$\dot{θ}=J^{-1}\dot{x}$

사실상 이렇게 도출된 $\dot{x}$에서 $\dot{θ}$로의 inverse kinematics만 있으면,  $\dot{x}$에서 $\dot{θ}$의 관계를 이용하여, $x$에서 $θ$의 계산이 가능하다. $x$에서 $θ$로의 간접적인 (approximation을 통한) 변환이 이 inverse kinematics의 핵심이다.

이 때, 현재의 $x$이 있으면 현재의 $θ$를 구할 수 (inverse kinematics of $x$ to $θ$) 있다는 말은 아님을 알아야 한다. 분명 이 kinematics는 우리 손에 없다.  $\dot{x}$에서 $\dot{θ}$의 관계의 inverse kinematics를 기반으로, 다음의 approximation 식을 도출할 수 있다.
 
$\Delta θ \approx J^{-1} \Delta x$

현재의 $x$의 위치를 다른 target 위치로 이동시키고자 한다면, 위의 식을 쉽게 이용할 수 있다.


<p align="right"> Hosung Nam <p>
