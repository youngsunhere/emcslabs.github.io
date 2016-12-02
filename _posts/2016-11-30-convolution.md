---
layout: post
title: Convolution
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

\begin{align}
(f * g )(t) & \, \stackrel{\mathrm{def}}{=}\ \int_{-\infty}^\infty f(\tau)\, g(t - \tau) \, d\tau \\
& = \int_{-\infty}^\infty f(t-\tau)\, g(\tau)\, d\tau.
\end{align}

- convolution은 두 함수 $$f(\tau)$$ 와 $$g(\tau)$$에 대해, 그 중 한 함수를 reverse하고, 즉 $$f(-\tau)$$ 혹은 $$g(-\tau)$$, 시간 축(t축)으로 -∞에서 +∞로 shift하면서 두 function의 pointwise 곱의 합(적분)의 함수다.
- t = 0 일때, $$f의\tau = g의\tau$$
- 두 함수의 pointwise 곱의 합 혹은 적분은 결국 상수값이다.
- convolution은 t의 함수이다.
- cross-correlation은 reverse를 생략한 convolution임.

## FFT
- FFT는 function의 pointwise 곱의 합(적분)이란 점에서 convolution과 유사하다.
- 1차원의 signal을 2차원 (complex plane) phasor인 z와 곱을 한 뒤 합을 한다. z-transformation라고도 부름.
- 선형대수의 inner product (1xN * Nx1)
- convulution 및 correlation과 다른 점은 이 둘은 시간의 함수이지만, FFT는 frequency의 함수.




<p align="right"> Hosung Nam <p>
