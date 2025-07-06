# Azure Custom Vision Project (250529, Lee Yeonmi)

## Project Overview
This project aims to develop computer vision models using Microsoft Azure Custom Vision.  
By leveraging transfer learning-based CNN models, it achieves high performance with a small amount of data while optimizing cloud resource usage.

## Key Technologies
- **Azure Custom Vision**: Main platform for AI model training and deployment  
- **Transfer Learning-based CNN**: Fine-tuning pre-trained models with limited data for fast and efficient training  
- **Computer Vision Architecture**:  
  - Image Classification: Static image input → CNN → Class probability output (Softmax)  
  - Object Detection: Bounding box + class prediction (SSD, YOLO family models)  
- **Automated Hyperparameter Tuning**: Utilizes Azure’s automatic tuning capabilities

## Practical Implementations
- Image classification  
- Object detection  
- Integration with external applications (REST API, Gradio interface)

## Evaluation Metrics
- **Precision**: The proportion of correct predictions among all predictions for a specific class  
- **Recall**: The proportion of actual class instances correctly identified by the model  
- **AP (Average Precision)**: The balanced average of Precision and Recall

## Key Results Summary
- The Rock model shows a good balance between Precision and Recall, with performance affected by the Probability Threshold  
- Bungee detection achieves accurate face detection when the threshold is above 11.2%  
- Fruit detection has low Precision for banana and orange, while Green Apple shows low probability due to insufficient training

## How to Run
- Test images via REST API calls  
- Adjust detection counts by changing the Threshold value in the Gradio app  
  Example: Threshold 0.5 → detects 2 objects, Threshold 0.8 → detects 1 object



# Azure Custom Vision 프로젝트 (250529, 이연미)

## 프로젝트 개요
본 프로젝트는 Microsoft Azure Custom Vision을 활용하여 컴퓨터 비전 모델을 개발하는 것을 목표로 합니다.  
전이 학습 기반 CNN 모델을 사용하여 적은 양의 데이터로도 높은 성능을 내고, 클라우드 자원의 효율적인 사용을 도모합니다.

## 주요 기술
- **Azure Custom Vision**: AI 모델 학습 및 배포 주요 플랫폼  
- **전이 학습 기반 CNN**: 사전 학습된 모델을 소량의 데이터로 미세 조정하여 빠르고 효율적인 학습  
- **컴퓨터 비전 구조**:  
  - 이미지 분류: 정적 이미지 입력 → CNN → 클래스별 확률 출력 (Softmax)  
  - 객체 탐지: 바운딩 박스 + 클래스 예측 (SSD, YOLO 계열 모델)  
- **자동 하이퍼파라미터 튜닝**: Azure 플랫폼에서 자동 조정 기능 활용

## 실습 항목
- 이미지 분류  
- 객체 탐지  
- 외부 프로그램 연동 (REST API, Gradio 인터페이스)

## 평가 지표
- **Precision**: 모델이 특정 클래스로 판단한 결과 중 실제로 맞는 비율  
- **Recall**: 실제 해당 클래스인 데이터 중 모델이 찾아낸 비율  
- **AP (Average Precision)**: Precision과 Recall의 균형을 나타내는 평균값

## 핵심 결과 요약
- Rock 모델은 Precision과 Recall의 균형이 우수하며, Probability Threshold 값에 따라 성능 변화 확인  
- Bungee 탐지는 Threshold가 11.2% 이상일 때 정확한 얼굴 탐지가 가능  
- Fruit 탐지는 바나나와 오렌지의 Precision이 낮고, Green Apple은 학습 부족으로 확률이 낮게 나옴

## 실행 방법
- REST API 호출을 통해 이미지 테스트 수행  
- Gradio 앱에서 Threshold 값을 조정하여 탐지 개수 변경 가능  
  예: Threshold 0.5 → 2개 탐지, Threshold 0.8 → 1개 탐지

