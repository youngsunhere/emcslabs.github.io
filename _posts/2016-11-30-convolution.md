---
layout: post
title: Convolutional Neural Network Gist
description: "Convolutional Neural Network"
headline: "Convolutional Neural Network"
categories: MACHINELEARNING
tags: 
  - Machine Learning
  - CNN
comments: false
mathjax: true
featured: true
published: true
---

## Convolution
- convolution은 두 function, f(x)와 g(x)에 대해, 그 중 한 function을 reverse하고, 시간 축(t축)으로 -∞에서 +∞로 shift하면서 두 function의 pointwise 곱의 합(적분)의 function이다.
- 두 함수의 pointwise 곱의 합 혹은 적분은 결국 상수값이다.
- convolution은 t의 함수이다.

## Cross-correlation
- cross-correlation은 reverse를 생략한 convolution임.
- FFT도 마찬가지이다.
	 - phase에 의한 artifact를 없애기 위해 1차원의 signal을 2차원의 phasor인 z와 cross-correlation시킴: z-transformation.


\begin{align}
(f * g )(t) & \, \stackrel{\mathrm{def}}{=}\ \int_{-\infty}^\infty f(\tau)\, g(t - \tau) \, d\tau \\
& = \int_{-\infty}^\infty f(t-\tau)\, g(\tau)\, d\tau.
\end{align}
