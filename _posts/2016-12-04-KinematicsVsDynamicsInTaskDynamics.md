---
layout: post
title: Kinematics vs. Dynamics in Task-dynamics
description: "Kinematics vs. Dynamics in Task-dynamics"
headline: "Kinematics vs. Dynamics in Task-dynamics"
categories: Math
tags: 
  - Jacobian
  - Linear Algebra
  - Kinematics
  - Dynamics
  - Task-dynamics
comments: false
mathjax: true
featured: true
published: true
---

## Kinematics vs. Dynamics in Task-dynamics

kinematics는 motion의 특징인 위치, 속도, 가속도 자체만이 그 연구 대상인 반면에, dynamics는 그 motion의 원리, 원인, 원천에 대한 연구이다.

forward kinematics는 joint의 motion 특징인 $θ, \dot{θ}, \ddot{θ}$으로부터 task의 motion 특징인 $x, \dot{x}, \ddot{x}$ 으로의 매핑이다.

$x = f(θ)$  
$\dot{x}=J\dot{θ}$  
$\ddot{x}=J\ddot{θ} +\dot{J}\dot{θ}$  

inverse kinematics는  task 변수 $x, \dot{x}, \ddot{x}$로부터 joint 변수 $θ, \dot{θ}, \ddot{θ}$ 으로의 매핑이다. 

$θ=f^{-1}(x)$  
$\dot{θ}=J^{-1}\dot{x}$  
$\ddot{θ} =J^{-1}(\ddot{x}-\dot{J}\dot{θ})$  

원래 robotics의 큰 흐름은 forward kinematics $\to$ inverse kinematics $\to$ dynamics $\to$ control theory이다.

dynamics는 position, velocity를 기반으로 force를 계산하는 방법으로, 주로 미분 방정식에 의해 정의된다. control하고자 하는 시스템에 대해서 정의하면 되는데, task나 joint space 모두에서 가능하다.

**Task-Dynamics**

forward kinematics  
$θ, \dot{θ}_{T=1}$ $\to$ $x, \dot{x}$  

dynamics  
$x, \dot{x}$ $\to$ $\ddot{x}$  

inverse kinematics  
$\ddot{x}$ $\to$ $\ddot{θ}$  
$θ,\ddot{θ}_{T=1}$ $\to$

integrate/solve  
$θ, \dot{θ}$ $,\ddot{θ}_{T=1}$ $\to$ $θ, \dot{θ}_{T=2}$  

$θ, \dot{θ}_{T=1}$ $\to$ $x, \dot{x}$ $\to$ $\ddot{x}$ $\to$ $\ddot{θ}$ $\to$ $θ, \dot{θ}_{T=2}$  


<p align="right"> Hosung Nam <p>
