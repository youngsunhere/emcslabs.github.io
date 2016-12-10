---
layout: post
title: Tensorflow Basics
description: "Fundamentals of Tensorflow"
headline: "Tensorflow Basics"
categories: MACHINELEARNING
tags: 
  - Machinelearning
  - Tensorflow
comments: false
mathjax: false
featured: true
published: true
---


# Tensorflow 

http://ferguson.tistory.com/1

# Tensorflow 기초


![DataFlowGraph]({{ site.url }}/images/dataflowgraph.gif)


- 텐서플로우는 기계학습과 딥러닝을 위해 구글에서 만든 오픈소스 소프트웨어 라이브러리  
- matlab의 simulink와 유사하게 building block 회로 설계하는 것과 유사한 visual programming language
- C++와 Python을 지원
- 데이터 플로우 그래프(data flow graph)를 이용해 수치계산(numerical computation)  
- 데이터 플로우 그래프란 **데이터**의 **흐름**과 **연산**을 node와 edge로 표현한 방향 그래프(directed graph)
- 데이터는 당연히 다차원 배열이고 **텐서**(tensor)라고 부르기에 텐서플로우라는 이름이 지어졌다
- 텐서플로우 설치 후 아래 커맨드를 실행하면 다음과 같은 설명을 볼 수 있다

~~~ shell
$ pip show tensorflow  
~~~

   > Name: tensorflow   
   > Version: 0.11.0  
   > Summary: **TensorFlow helps the tensors flow**  

---
<br />

## 기본 용어

<br />

### 오퍼레이션 (Operation)

- 그래프 상의 노드는 오퍼레이션으로 불린다
- 오퍼레이션은 하나 이상의 텐서를 입력으로 받아 연산을 수행하고 결과를 반환

### 텐서 (Tensor)

- 내부적으로 모든 데이터는 텐서를 통해 표현
- 그래프 내의 오퍼레이션 간에는 텐서만이 전달된다 (Caffe의 Blob과 유사)

### 세션 (Session)

- 그래프를 실행하기 위해서는 세션 객체가 필요
- 세션은 오퍼레이션의 실행 환경을 캡슐화한 것
- 오퍼레이션을 세션 안에 넣어 실행시킨다고 생각하자

### 변수 (Variables)

- 변수는 그래프의 실행시, 패러미터를 저장하고 갱신하는데 사용
- 메모리 상에서 텐서를 저장하는 버퍼 역할을 한다

---
<br />

## (거의) 모든 것은 operation !

<br />

다음 예제들을 통해 텐서플로우와 친해져보도록 하자

### 예제 1

~~~ python
import tensorflow as tf

# hello라는 상수 정의
hello = tf.constant("Hello, World")

# 세션 정의
sess = tf.Session()

# 세션 실행 결과 출력
print sess.run(hello)
~~~

<br />

### 예제 2
~~~ python
import tensorflow as tf

# tf 세션 정의
sess = tf.Session()

# 생성자가 리턴하는 값을 출력으로 하는 constant operation a와 b를 정의
# 상수 a, b 정의가 아닌 operation a, b의 정의라고 생각하자
a = tf.constant(2)
b = tf.constant(3)

# c는 operationa와 a와 b를 더하는 operation
# a+b를 계산해 c에 대입하는 것이 아님
c = a + b

# 다음을 실행하면 5가 아닌, "Tensor("add:0", shape=(), dtype=int32)"을 출력
print c

# 세션 실행 결과를 출력
print sess.run(c)
~~~

<br />

### 예제 3
~~~ python
import tensorflow as tf

# 변수를 0으로 초기화
state = tf.Variable(0, name="counter")

# state에 1을 더하는 operation 정의
a = tf.constant(1)
new_state = tf.add(state, a)
update = tf.assign(state, new_state)

# 그래프를 생성하기 전에 변수를 초기화해야만 한다 - init_op 정의
init_op = tf.initialize_all_variables()

# 그래프를 띄우고 오퍼레이션들을 실행
with tf.Session() as sess:
    # 초기화 오퍼레이션 실행
  sess.run(init_op)
    # state의 초기 값을 출력
  print(sess.run(state))
    # session 실행, state 값 출력
  for _ in range(3):
    sess.run(update)
    print(sess.run(state))

# 0, 1, 2, 3 이 출력된다
~~~

---

<p align="right"> Sung Hah Hwang, Hosung Nam </p>


