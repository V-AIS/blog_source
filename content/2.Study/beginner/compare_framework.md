---
title: 프레임워크 별 장단점
tags: 
  - Deep Learning Framework
# draft: true
---

이 글은 드래프트 입니다.

{{< columns >}}
## TensorFlow
### 장점  
- 성숙한 에코시스템, 강력한 지원과 다양한 도구, 라이브러리 제공  
- TensorFlow Serving, TensorFlow Lite 등을 통한 모델 배포 용이성  
- 연구와 산업 분야 모두에 적합

### 단점  
- 모델 설계 및 실험을 위한 유연성이 상대적으로 부족할 수 있음  
- 처음 사용자에게는 기능과 API의 복잡성이 높을 수 있음

<--->

## PyTorch
### 장점  
- 쉬운 문법과 직관적인 설계로 사용자들에게 인기  
- 동적 그래프 형태로 자유로운 모델 디자인 및 실험 가능  
- 활발한 커뮤니티와 개발자들의 지속적인 기여로 발전 중

### 단점  
- TensorFlow보다 기업에서의 지원이 상대적으로 부족할 수 있음  

<--->

## Keras
### 장점  
- 직관적이고 간단한 API로 빠른 프로토타이핑 가능  
- TensorFlow, Theano, CNTK 등 다양한 백엔드 지원. (추후 추가 예정)
- 초보자와 교육 목적으로 적합한 사용자 친화적인 환경

### 단점  
- TensorFlow나 PyTorch에 비해 저수준 기능을 제어하기 어려울 수 있음  
- TensorFlow나 PyTorch에 비해 모델 수정 및 실험에 제한이 있을 수 있음
{{< /columns >}}
