# CNNModelAnalysis

### 내용
    CNN 모델에 Accuracy, Training Loss Curve 형태를 기준으로 여러 기법 적용 성능 비교 분석

### 데이터셋
    CIFAR-10

### 목적
    - Baby Sitting의 중요성 상기
    - Pytorch 모델 구현 연습
    - Batch Normalization, Weight Initialization, Dropout 등 기법 적용 커스터마이징
    - GridSearch 구현 및 하이퍼파라미터 튜닝 후 주요 하이퍼파라미터 확인 및 직관 터득하기

### 결과(직관적)
    - Batch Normalization : 이상적인 학습 Loss Curve의 형태처럼 초기 급격히 떨어지다가 이후 완만히 Loss 0으로 수렴토록 해줌
    - Dropout : Loss Curve의 기울기 형태가 조금 더 완만한 형태로 만들어줌(과적합 방지 효과)
    - Weight Initialization : BN, Dropout에 비해 크게 성능에 이바지하는 형태는 아님. 타 주요 기법을 우선 적용 후 추가 성능개선을 위해 여러 Initialization 기법을 활용하는 편이 좋을 듯
    - Learning Rate : 가장 우선적으로 안정적인 Loss Curve형태를 잡아주는 범위를 찾아야함
![image](https://user-images.githubusercontent.com/69191799/128672283-1316594b-9699-421f-91cb-7618aed9e50e.png)

