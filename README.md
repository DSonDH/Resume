## 소개
![프로필이미지](https://github.com/SonDooHwan/Resume/blob/master/images/SonDooHwan_200x200.jpg)
- 이름: 손두환
- 현) (주) UST 21 부설연구소 데이터본부 인공지능팀 (~ 25-08-31)
- 군필여부: 석사전문연구요원 복무만료 
- Email: ensl940120@naver.com

```
높은 퍼포먼스 및 설명 가능한 머신러닝 개발을 지향하고 있습니다.
현재는 주로 시계열예측 연구를 수행하고 있고, 해양AI 프로젝트 추진 시 발견한 여러 난제 해결에 관심을 두고 있습니다.
(Explainability, Causality, OOD, OD, Multimodality, Spatiotemporal Interpolation, etc.)
```

## 이력
- 고려대학교 바이오의공학과 졸업(2013.03 ~ 2017.09)
- 고려대학교 바이오융합공학과 졸업(2017.09 ~ 2020.08)
- 현) UST21 ([Underwater Survey Technology 21](https://www.ust21.co.kr/), 2020.09 ~ 2025.8)
- (~2025.09 : 박사과정 진학 희망)

## 사용 기술
최신 머신러닝 기술, 통계 기법들을 구현하고 검증할 수 있을정도의 코딩 스킬을 가지고 있습니다.<br/>
다양한 이미지 처리 기술 보유.<br/>
다양한 시계열 딥러닝 모델 구현 및 튜닝 경험 보유.<br/>
다양한 통계 기법 적용 능력 보유.<br/>
- Python
- Pytorch
- MATLAB

## 연구 경험

### 논문
- Jin Myoung Seok,Wanzee Cho,Doo-Hwan Son,Jong Hwa Shin,Eun Bin Cho,Sung Tae Kim, Byoung Joon Kim,Joon-Kyung Seong,Ju-Hong Min, "Association of subcortical structural shapes with fatigue in neuromyelitis optica spectrum disorder", SCIENTIFIC REPORTS, (2022)
- Doo-Hwan Son,Minki Chun,Young Taeg Kim,Boonsoon Kang,Kuk Jin Kim,Jin Hyun Han, "FogFusionNet: Coastal Sea Fog Prediction by Using a Multimodal Deep Learning Approach", IEEE ACCESS, (2024)

### 프로젝트
**@ UST21 (20-09-01 ~ 25-08-31)**  
**해양예측정보 종합분석 및 특화 해양예보**, 국립해양조사원 예보과 (2023-09 ~ 2025.08) 
- 3차원 해수 프로파일 예측 (ConvLSTM 활용)
- 단기 조위 예측을 위한 데이터 분석 (해양 기상 시계열 관측자료 수집, 전처리, 결측보간, Utide, Wavelet Transform, Cross Correlation 알고리즘 활용 분석 수행), 인공지능 모델 개발 및 고도화 (LightGBM, PatchTST, 등 응용), 현업화 디자인

**항계안전 해양정보 제공 확대 및 개선**, 국립해양조사원 예보과 (2020-09 ~ 2023.12)
- 해무관측 CCTV 및 시계열 관측자료 분석, 인공지능 모델 입력자료 고도화
- 인공지능 기반 (Tree기반 ML모델, ensemble 모델, classifier vision모델) 해무 판별, 예측모델 개발 및 고도화
- 멀티모달 해무판별 및 예측 모델 개발

NIA_인공지능 학습용 데이터구축 사업_이안류 CCTV 데이터, 한국지능정보사회진흥원 (2022-05 ~ 2022-12)
- 이안류 이미지 자동라벨링 알고리즘 개발
- 이안류 탐지 및 예측 모델 개발 

NIA_인공지능 학습용 데이터구축 사업_해무안개 CCTV 데이터, 한국지능정보사회진흥원 (2021-06 ~ 2021-10)
- 라벨링 방법론 수립 기여
- 해무 판별 및 멀티모달 해무 예측 모델 개발 
<br/>

@ 석사과정 <br/>
멀티모달 뇌 영상 기반 예후 판별법 개발  
- BRATS 2015 데이터를 사용하여 Inception V3 네트워크로 High grade glioma, Low grade glioma 구분 학습  
- 학습된 딥러닝 모델의 latent 특징 벡터를 환자별로 추출  
- 각 환자의 특징을 평균하여 최종 특징 벡터 생성  
- 환자별 특징 벡터와 비교 후 Louvain method를 적용 → 통계적으로 유의미한 survival 양상 차이 확인  

딥러닝을 활용한 뇌 병변 부위 자동 추출및 이를 활용한 classification <br/>
- 멀티 모달리티 이미지 정합 및 전처리들을 통해 딥러닝 모델의 입력 이미지 생성
- 뇌경색 부위 추출, 뇌종양 부위 추출, white matter hyperintensity 부위 추출 (U-net모델)
- 원발성 뇌암, 뇌전이암의 뇌종양 부위 segmentation (U-net모델)
- 추출한 뇌종양 label에서 feature vector 생성 후 이를 활용한 원발성뇌암/뇌전이암 classification 진행, 정확도 0.85 달성 <br/>

NMOSD환자, MS환자의 fatigue score, subcortical shape mesh를 활용한 statistical analysis <br/>
- NMOSD: Neuromyelitis Optica Spectrum Disorder, MS: Multiple sclerosis
- 목적: Samsung Medical Center의 NMOSD, MS환자의 Fatigue score와 T1 brain MRI데이터를 사용하여 fatigue score와 significant한 correlation을 보이는 sub-cluster 추출
- T1 이미지에서 brain parcellation을 진행하고, 3D mesh surface를 추출하고 surface를 registration한 후 vertext별 정보를 추출하기 위해 local-shape-volume 계산
- vertex별 local shape volume과 fatigue score와의 partial rank correlation분석을 진행하고, Cluster-based-statistics를 활용하여 통계적으로 유의미한 subcluster를 추출하여 가시화
- 가시화 한 subcortical 별 sub-region들에 대한 임상적 해석을 통해 fatigue와 관련한 NMOSD, MS환자의 좀더 local한 연관부위를 찾음

## patent
- (등록) 김국진, 김봉국, 한진현, 손두환, 곽경일, 이준호, "Method for predicting rip current using observation data based on artificial intelligence and apparatus thereof", KR-Registration No. 10-2588415-0000  
- (등록) 김국진, 김봉국, 한진현, 손두환, 이석호, "Method for detecting rip current using CCTV image based on artificial intelligence and apparatus thereof", KR-Registration No. 10-2602439-0000  
- (등록) 김국진, 김봉국, 한진현, 손두환, 김영택, 임채호, "Method for discriminating sea fog using image based on artificial intelligence and apparatus thereof", KR-Registration No. 10-2460705-0000  
- (출원) "딥 러닝 네트워크 기반 멀티 MR 이미지를 활용한 원발성뇌암 뇌전이암 구분 방법", 성준경, 손두환, KR Patent 10-2020-0065178 (2020)  
- (출원) "딥 러닝 기반 멀티 MR 이미지의 이미지 특징을 활용한 환자 예후 예측 방법", 성준경, 손두환, 김정훈, KR Patent 10-2020-0065249 (2020)  
---
읽어주셔서 감사합니다. <br/>
부족한 부분이나 더 궁금하신 내용이 있다면 [이슈](https://github.com/SonDooHwan/Resume/issues)로 남겨주시거나, ensl940120@naver.com 으로 연락주세요.<br/>
감사합니다.

