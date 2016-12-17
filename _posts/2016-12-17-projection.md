---
layout: post
title: Projection
description: "Projection"
headline: "Projection"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Projection

- Projection이란, 벡터 v에 손전등을 비추어 어떤 subspace에 그림자가 생기도록 하는 것이다.
	- 손전등의 불빛 방향과 subspace가 수직을 이루면 orthogonal projection.
	- 수직을 이루지 않으면 nonorthogonal(=oblique) projection.
	- projection은 하나의 공간을 두 개의 부분공간 decompose한다. <br>
	  1) v의 그림자가 생기는 subspace <br>
	  2) v가 project되는 방향과 일치하는 subspace
<br>
- projection은 어디에 쓰이나?
	1. linear regression
		- 데이터 A와 b를 가지고 선형 방정식 Ax=b의 해를 구하려 하는데,데이터 내에 오류가 있으면 해를 구할 수가 없다. 
		- 따라서 데이터 원본을 **가장 덜 손상**시키면서도 **해를 구할 수 있게** 데이터를 변형해야 한다. 
		- 변형방법: range(A)에 b를 project함 -> b의 그림자와 에러, 그 둘로 쪼개짐
	2. 각종 decomposition의 핵심 도구
		- QR decomposition 
		- Singular Value Decomposition
		- Eignevalue Decomposition
<br>
- projector P in general (orthogonal/nonorthogonal projection에 모두 해당)
	- range(P)에 projection 수행.
	- Pv <br>
	  = v projected onto the column space of P. <br>
	  = range(P)에 비친 v의 그림자.
	- square matrix
	- symmetric matrix
	- not always orthogonal matrix
	- P<sup>2</sup>=P (<--idempotent)
	- m-by-m P는 m차원 공간을 원점 밖에 공유하지 않는 complementary 관계의 두 subspace로 분해시킴. 
		1. range(P) <br>
		   = null(I-P)<br>
		   = v의 그림자가 비춰지는 subspace
		2. null(P) <br>
		   = range(I-P)<br>
		   = residual vector Pv-v 가 들어있는 subspace<br>
		   = range(P)에는 Pv-v의 그림자가 절대 안 생김.
<br>
- orthogonal projector P
	- range(P)에 수직으로 projection 수행.
	- P = P<sup>T</sup>
	- range(P)&perp;null(P) <br>
	  = the column space of P is equal to the row space of P  <br>
	  -> symmetric matrix이기 때문
	- rank = 1

<br>

- orthogonal projector P 공식
	- 벡터 b를 벡터 a 위에 project 하는 P<br>
	  $p = a{a^\mathrm{T}b \over a^\mathrm{T}a}$<br>
	  1) a<sup>T</sup>b: b를 a에 project하고 a길이만큼 scale<br>
	  2) a<sup>T</sup>a: a길이만큼 unscale<br>
	  $P = {aa^\mathrm{T} \over a^\mathrm{T}a}$<br>
	  projection matrix는 a의 외적/내적
	  
	- 벡터 b를 range(A)에 project 하는 P<br>
	  $P = A(A^\mathrm{T}A)^\mathrm{-1}A\mathrm{T}$<br>
	  
	
	
	
<p align="right"> Yeonjung Hong <p>
