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

Forward Kinematics를 이용하여 주어진 Joint angle로부터 2 Link SCARA Robot 말단부의 위치를 계산할 수 있었습니다.
로봇 말단부의 위치 말고 속도는 어떻게 될까요? 
위의 식에서 x2 와 y2를 시간 t에 대해 미분하면 되겠죠 뭐 ㅋ
x2는 θ1과 θ2의 함수이구요 θ1과 θ2는 다시 시간 t의 함수입니다.
독립변수가 여려개인 함수를 미분하실 때에는 편미분과 chain rule을 사용하시면 됩니다요~
End-effector의 속도와 Joint의 각속도의 관계를 나타내는 편미분 된 Matrix를 Jacobian matrix
Jacobian matrix가 full rank가 아닌 경우나 singular (det(J)==0) 인 경우를 제외하고는 
항상 End-effertor의 속도를 결정하는 Joint 각속도를 계산할 수 있습니다.
Full rank가 아닌경우 즉 Jacobian matrix가 square matrix(행, 렬의 개수가 같은 정사각형 행렬)가 아닌 경우는 
