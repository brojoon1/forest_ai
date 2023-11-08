# GRIN (Greenery Recovering AI solutioN)
- 인공위성 이미지를 활용한 AI기반 제주도 불법 산림 훼손 탐지 솔루션

## 프로젝트 개요
- 미래 내일 일 경험 사업 제안 프로젝트
- 데이터: 인공위성 이미지 데이터
- 프로젝트 기간: 2023/10/9 ~ 2023/10/25
- 팀원: AI 개발 2명 / DX 3명

## 주제 선정 배경

![Untitled (14)](https://github.com/brojoon1/AI_detection_of_illegal_forest_damage/assets/81418195/c3542a6d-532f-4266-8150-0e7d75f2d603)
- 위성 이미지 데이터 시장 규모 확장과 국내 산림 위성 개발 및 인프라 구축 전망
    - 위성 이미지 데이터 규모는 8조('21년)에서 21조('26년)으로 약 3배 성장 예상
    - 국내에서 주기적인 산림 변화 모니터링, 신속한 산림 재난 대응을 목적으로 2025년 산림 위성 개발 및 발사와 국가 산림 위성 정보 활용 센터 구축을 추진 중
<br></br>

![Untitled (15)](https://github.com/brojoon1/AI_detection_of_illegal_forest_damage/assets/81418195/4fa28609-49d5-43e5-8847-995ecbd5da27)
![Untitled (16)](https://github.com/brojoon1/AI_detection_of_illegal_forest_damage/assets/81418195/757392dd-9f0e-4b60-a5ce-dbd944fcf6a5)

- 제주도 전 지역이 생물권보존구역임에도 지속적인 불법 산림 훼손 발생
    - 제주도는 2019년 6월 이후로 전 지역이 생물권 보존 구역으로 지정됨
    - 이런 상황에도 불구하고 불법 산림 훼손이 증가하고 있으며, 곶자왈이 3년 동안 26만여의 넓이가 훼손됨에도 불구하고 탐지 및 조치가 미비함

## 프로젝트 상세 설명
### 1. 활용 데이터
- AI Hub의 ‘산림수종 이미지(강원 및 충청)’ 데이터 사용
https://www.aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=data&dataSetSn=135

### 2. 모델
- 정상 지역(normal)과 불법 산림 훼손 의심 지역(abnormal) 이미지 분류
    - VGG16 모델 사용

- VGG16 모델로 분류된 abnormal 이미지를 객체 탐지
    - YOLOv5 모델 사용

### 3. 웹 배포
- Streamlit (현재는 배포 중지)

## 기대 효과 및 활용 분야
### 1. 기대효과
- 준공 후, 1, 2, 5, 10년 차에만 시행하던 모니터링을 수시로 확인 가능
- 상시 모니터링을 통한 훼손 구역 탐지 및 대응 속도 향상
- 전수조사에서 훼손이 탐지된 구역만 조사하는 방식으로 바꿔 담당자 부담감 감소
### 2. 활용분야
- 제주도에서 대한민국 전국으로 사업구역 확대 가능
- 자율주행 드론 등을 활용하여 훼손 현장에 직접 방문 없이 업무 처리 가능
- 불법야적장, 선박, 밀입국 등 다른 분야의 솔루션에서 활용 가능

## 개발툴 및 방법
- Git hub
    - 형상관리
- Figma
    - UX/UI 프로토타입 제작
- Google Drive
    - 공유 드라이브를 생성하여 데이터, 모델, 문서 등 파일 관리
- Google Colab
    - 이미지 분류와 객체 탐지

## 팀 구성원 및 담당 역할
- Leader 
    - 조재성
        - 팀장, 솔루션 흐름도, 서비스 구성도, IT인프라 구성, 발표
- AI 개발
    - 김형준
        - 데이터 수집 및 AI 모델 개발, Streamlit 웹 제작
    - 정은찬
        - 데이터 수집 및 AI 모델 개발, Figma 프로토 제작
- DX 
    - 김민주
        - 환경 분석, 제안 전략, PPT 작성
    - 한수빈
        - 제안 기획, 기대효과, 향후계획, PPT 작성