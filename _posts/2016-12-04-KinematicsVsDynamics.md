---
layout: post
title: Kinematics vs. Dynamics
description: "Kinematics vs. Dynamics"
headline: "Kinematics vs. Dynamics"
categories: Math
tags: 
  - Jacobian
  - Linear Algebra
  - Kinematics
  - Dynamics
comments: false
mathjax: true
featured: true
published: false
---

## Kinematics vs. Dynamics

kinematics는 motion의 특징인 위치, 속도, 가속도 자체만이 그 연구 대상인 반면에, dynamics는 그 motion의 원리, 원인, 원천에 대한 연구이다.

forward kinematics는 joint의 motion 특징인 $θ, \dot{θ}, \ddot{θ}$으로부터 task의 motion 특징인 $x, \dot{x}, \ddot{x}$ 으로의 매핑이다. 특히, $θ$로부터 $x$로 

$x = f(θ)$
$\dot{x}=J\dot{θ}$
$\ddot{x}=J\ddot{θ} +\dot{J}\dot{θ}$  

inverse kinematics는  task 변수 $x, \dot{x}, \ddot{x}$로부터 joint 변수 $θ, \dot{θ}, \ddot{θ}$ 으로의 매핑이다. ($x$에서 $θ$로의 inverse는 구할 수 없음)

$\dot{θ}=J^{-1}\dot{x}$
$\ddot{θ} =J^{-1}(\ddot{x}-\dot{J}\dot{θ})$

Dynamics는 말그대로 힘에 관련된 이야기이다. Kinematics에서는 힘은 전혀 고려하지 않고, 그냥 각도만 가지고 이야기한다.

<p align="right"> Hosung Nam <p>
