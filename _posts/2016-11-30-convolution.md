---
layout: post
title: convolution
date: 2016-11-30
tags: convolution
---
convolution은 두 function, f(x)와 g(x)에 대해, 그 중 한 function을 reverse하고 시간 축으로 -∞에서 +∞로 t축을 따라 shift하면서 두 function의 pointwise 곱의 합(적분)의 function이다. 그래서 합 혹은 적분은 상수값이어야하는데, convolution은 t의 함수이다.

cross-correlation은 reverse를 생략한 convolution임. FFT도 마찬가지이다 (phase에 의한 artifact를 없애기 위해 1차원의 signal을 2차원의 phasor인 z와 cross-correlation시킴: z-transformation)