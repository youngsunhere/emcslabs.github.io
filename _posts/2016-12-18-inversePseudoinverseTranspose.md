---
layout: post
title: Inverse, Pseudoinverse, Transpose
description: "Inverse, Pseudoinverse, Transpose"
headline: "Inverse, Pseudoinverse, Transpose"
categories: Math
tags: 
  - Math
comments: false
mathjax: true
featured: false
published: true
---

## Transpose, Inverse, Pseudoinverse 

- m-by-n A
	- A의 row space에 있는 벡터를 column space로 transform

- n-by-m A<sup>T</sup>
	- A의 column space에서 row space로 공간은 transform
	- 하지만 column space에 있는 벡터를 row space로 transform하는 것까지는 못함

- m-by-m A<sup>-1</sup>
	- rank=m=n일 때만(full rank & square), 역행렬 존재.
	- nullspace에 원점 밖에 없는, nonsigular 행렬. <br>
	  = 원점으로 transform시킬 수 있는 벡터는 0벡터뿐.
	- A의 column space에 있는 벡터를 row space로 transform 할 수 있음. 

- A<sup>T</sup>=A<sup>-1</sup>
	- A가 orthogonal matrix일 때, A<sup>T</sup>=A<sup>-1</sup>가 성립한다. 
		- orthogonal matrix 
		  1. orthonormal columns로 이루어짐 
		  2. square matrix
		- Tip1. orthogonal 벡터들은 linearly independent
		- Tip2. orthonormal vectors = orthogonal unit vectors
   - orthogonal projector P
       - P = P<sup>T</sup> = P<sup>-1</sup>
       - PP<sup>T</sup> = P<sup>T</sup>P = I
       - P의 column space = row space
- n-by-m A<sup>+</sup>
	- A가 singular 행렬일 때, A<sup>-1</sup>의 대체물이 A<sup>+</sup>
	- column space에서 row space로 transform 할 수 있는 벡터들에 한하여 inversion 수행
	- left nullspace에 있는 벡터들은 내버려 둠
	
	
<p align="right"> Yeonjung Hong <p>