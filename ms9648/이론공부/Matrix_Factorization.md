---
layout: post
title: "Math Factorization"
authors: [ms9648]
tags: ["머신러닝", "선형대수학", "추천시스템"]
description: "MF기반 Collaborative Filtering을 공부하다가 정리하였습니다.  Matrix Factorization With Rating Completion: An Enhanced SVD Model for Collaborative Filtering Recommender Systems를 읽고 SVD, RSVD, ESVD에 대해 정리하였습니다."
post-image: ../assets/images/post-Matrix-Factorization/SVD.PNG
featured: true
use_math: true
---

# SVD(Singular Value Decomposition, 특잇값 분해)
![image](../assets/images/post-Matrix-Factorization/SVD.PNG)

행렬을 특정한 구조로 분해하는 방식입니다.

## LU Factorization
선형대수학 수업시간에 배웠던 LU Factorization 개념과 비슷하게 생겼습니다.

LU Factorization은 Linear system에서 $Ax = b$의 해를 구하는 방법입니다.

LU Factorization을 간단히 나타내면 다음과 같습니다.

$ \mathbf{A} = \mathbf{LU} $

$ \mathbf{A}\mathbf{x} = b → \mathbf{LU}\mathbf{x} = b $


행렬 A를 LU로 분해하는 방법으로, L은 하삼각행렬, U는 상삼각행렬입니다.
L은 대각선 성분이 모두 1이고, 그 위는 전부 0, 그 아래는 non zero인 단위하삼각행렬입니다.
U는 

## Matrix Factorization(MF)