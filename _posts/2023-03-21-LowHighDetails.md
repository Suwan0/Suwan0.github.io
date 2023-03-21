---
title: "Low level details와 High level semantics"
date: 2023-03-21 18:51:00 -0400
categories: jekyll update
---
이번 post에서는 Low level details와 High levels semantics의 구분 방법을 알고 각각에 대해서 정리해보자.

## Low level details와 High level semantics
- Low level details와 High level details(semantics)구분 방법
    - Abstract가 더 됐나 덜 됐나의 차이이다.
    - 그럼 abstract란 무엇일까?
        - 컴퓨터 비전에서는 시각 정보를 표현하거나 이해할 때 개념적 복잡성 또는 일반화 수준을 나타낸다.
        - 즉 더 넓은 맥락, 관계 혹은 의미를 말한다.
        - 딥러닝에서는 abstact하다는 것은 일반적으로  deep layer에서 추출한 High level semantics를 의미하고 객체와 이미지의 맥락을 이해하는데에 도움이 된다. 덜 abstact한 특징은 specific details and local patterns에 초점을 맞춘다.

![Untitled (1)](https://user-images.githubusercontent.com/122383307/226571611-ecde0ef2-4e19-4543-9cd8-f3b9b00bca59.png)

- Low-level feature
    - 이미지의 색이나 경계(edge) , corners, texture등을 의미한다.
    - deep learning model에서 early layer에서 추출한다.
    - Image의 local structure와 pattern을 이해하는데 도움이 된다.
    - Semantic segmentation에서는 fine-grained information(objects와 regions이 비슷할 때 구분해주는 정보)을 추출해내는 데에 있어서 중요하다.
- High level sematics
    - Image의 추상적인 것과 global features를 의미한다.
    - deep layer에서 추출한다.
    - 객체들을 recognizing하고 다른 것들과의 관계를 파악한다.
    - 이미지의 전반적인 의미나 objects를 판단하는 데에 도움이 된다.
    - 다른 object class들을 분류하고 정확한 segmentation image를 얻는데에 중요한 요소이다.
