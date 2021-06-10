# WithMe_AI

설명

## 진행 상황

### 5/17
- 꽃 이미지 분류 인공지능 딥러닝 예제를 실행해보면서 overfitting나서 validation-auccracy가 이상하게 나오길래 validation-auccracy에 대해서 찾아 봤다. 그리고 드롭아웃을 해보니까 vlidation accuracy가 정상적으로 잘 나왔다.
- [꽃 이미지 분류 딥러닝](https://www.tensorflow.org/tutorials/images/classification?hl=ko)
- [Validation-Accuracy관련에 찾아본 사이트](https://roy881020.tistory.com/entry/validation-accuracy-%EC%A0%80%ED%95%98trainingvalidationtest-dataset)

### 5/18
- [YOLOv4, roboflow관련 사이트 꼭 실행해보기](https://blog.roboflow.com/training-yolov4-on-a-custom-dataset/)
- 구글에서 욜로에 대해서 찾아보던중에 위에 사이트가 가장 따라하기 쉽고 그 사람에 개발환경도 mac이 어서 좋았다. 이따가 방과후에 3090에서 실행해봐야겠다.

### 5/ 20
- 위에 유튜브에서 yolov4강의를 따라하면서 전처리 까지 했다.
- 다음 시간에는 모델학습을 할것이다.

### 5/21
- 스택 예선에 붙었다. 기분이 매우 몹시 좋다.
- [시각적주의가 있는 이미지 캡션](https://www.tensorflow.org/tutorials/text/image_captioning?hl=ko#download_and_prepare_the_ms-coco_dataset)을 실행해 보면서 토큰화라는 단어를 발견하게 되었다. 예전에 지나가다가 한번씩 봤었는데 이번기회에 자세히 알아보고자 토큰화에 대해서 알아보겠다.
- [토큰화](https://wikidocs.net/21698)

### 5/24
- 학교 컴퓨터에 yolov4 설치 하고 실행 하기 까지 완료했다.(anydesk를 사용했다.) [yolov4 모델 깃](https://github.com/theAIGuysCode/yolov4-deepsort)
- 피피티를 어떻게 만들지 구상하였다.
  * 개선 서비스 :  이미 나와있는 서비스와 다른 점(차별 점)  강조
  * NUGU Play Kit(https://developers.nugu.co.kr)을 충분히 숙지하고 실현 가능한 서비스로 구체화
  * 현재 사용자 경험의 문제점 및 제안 서비스 적용 시 사용자 효용을 명확히 제시
  * 서비스 컨셉, 주요 기능 및 서비스 시나리오(음성) 구체화
  * 사용자 발화 주요 의도(Intent) 및 이에 대한 음성의 반응을 상세히 설명
  * 외부 API 연동 시 API의 기능과 연동구조를 설명
    
### 5/25
- 스택 본선에서 발표할 내용을 정리 하였다. 
- yolov4를 실행하여 결과를 확인 했지만 아직 정확도가 부족한것이 많았음.
- 나중에 더 연구 해보겠다.

### 5/27
- 피피티 만들 기획서 다썻다.
- [이미지 캡션 논문](https://arxiv.org/pdf/1502.03044.pdf)이미지 캡션하기 위해서 논문을 참고 했다. 
- [이미지 데이터 셋](http://images.cocodataset.org/annotations/annotations_trainval2014.zip)
- [이미지 데이터 셋](http://images.cocodataset.org/zips/train2014.zip)

### 5/ 27
- 시각장애인과 면담을 하러 장애인 센터에 가서 면담을 했다.

### 5/29 ~ 30
- jupyter notebook에서 직접 실행시켜 학습을 시켰지만 cpu만 사용해서 gpu설정하다가 오류가 났었다.
- 실행 당시 버전
- cuDNN v8.0.5
- CUDA 11.1
- cudnn 초기화가 안됨


- UDA 11.0은 gpu인식을 못함

### 5/30
- 학교 컴퓨터 cuda 환경 맞춤 하지만 컴터 에 cuda가 잘 안먹는데 글카 3090이 좀 안맞는다

### 6/1
- 스택 발표 자료 조사 및 발표 대본 씀
- 시각장애인 보조 기구 자료 조사 더 찾아볼것


### 6/3
- 스택 ppt에 추가할 내용 정리

### 6/4
- 쿠다 환경 세팅 함

### 6/7
- 지금까지 했던 거 중간 점검 함 
- 중간 점검 내용
- 서비스 시나리오
- 영상편집(다빈)한 것을 처음에 보여주고 우리가 구현할 것을 설명해주기

- 파트별도 구현된것
- 앱 : 카메라
- Ocr : x
- img_caption : x

- 파트별로 구현되지 않은 것
- 앱 : 사진찍는거, 서버통신, 누구연결
- Ocr : 데이터 못모았고 훈련 코드 못짬
- img_caption : 컴터 gpu세팅이 안됨

- 6/19일 발표 전까지 구현 가능한 것
- 앱 : 해상도 줄이는 기능(최적의 해상도 사이즈 찾기), 서버 통신
- Ocr : ocr기능 
- img_caption : 포맷하고 나서 2080컴에 세팅하면 바로 가능합니다.


- 문제가 뭐냐
- 안드로이드 버전 4.4에 지원하는 라이브러리가 없어서 하드웨어에 있는 카메라제어가 힘듬

- 로드밸런싱 구축하기가 힘듬

### 6/8
- 3090 컴퓨터 쿠다 설치 안되서 2080 포맷하고 나서 세팅함 
- 하지만 실패 했다.(우분투와 window에서 둘다 해봤는데 안된다.)
- 서비스 시나리오에 쓸 영상 만듬

