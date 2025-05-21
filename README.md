# 건설용 자갈 암석 종류 분류 AI 경진대회 

### 1. Abstract

- [건설용 자갈 암석 종류 분류 AI 경진대회](https://dacon.io/competitions/official/236471/overview/description)
- Task: Classification
- Domain : 건설용 자갈 이미지 / 질감 기반 분류
- Objective : 자갈의 표면 질감을 기반으로 7개의 클래스 분류
- Evaluation : Macro F1
- Dataset
  - Train : 380,020장의 RGB 이미지
  - Test : 95,006장의 RGB 이미지
- Challenge
  - 일부 모델이 자갈의 Edge에 의존하는 경향
  - 질감 중심으로 분류할 수 있는 방법 필요
- Approach
  - 질감 손실 없는, 질감을 더 표현할 수 있는 Augmentation 적용
  - CNN 기반 ResNet152 -> DensNet121 -> DenseNet + CBAM
  - 추가 ViT 모델 적용 (TBD)
- Key Findings
  - 증강 없이 베이스 모델이 ResNet을 사용했을 경우, 데이터에 따라 모델이 Edge 영역에 집중하는 경우가 있음
- Result
- Takeaway

