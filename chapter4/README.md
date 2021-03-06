# 4장. 텐서플로 라이트 모델 개발


## 4.1 텐서플로 라이트 모델 개발 워크플로

<img src="img.png" width="50%" height="50%">

### 4.1.1 모델 선택
- 개발하고자 하는 솔루션이나 서비스에 적합한 모델을 선택하자
- 모델 개발에는 텐서플로를 이용하고, 모델 변환 및 최적화에는 텐서플로 라이트를 이용한다.
- **이미 개발된 모델은 텐서플로나 텐서플로 허브에서 찾아볼 수 있다.**

### 4.1.2 모델 변환
- TensorFlow Lite Converter
- .tflite 파일로 변환하는 과정에서 자동으로 최적화를 한다.
- 정확도 손실을 최소한으로 하면서 모델의 크기를 줄인다.

### 4.1.3 기기 배포
- 프로젝트 안에 .tflite 파일을 직접 넣어서 모델을 사용할 수 있다.
- 런타임으로 백엔드 서버에서 제공받을 수 있다.

### 4.1.4 모델 최적화
- 실행 속도나 정확도를 더욱 개선하기 위해 직접 최적화 가능하다.
- **모델의 정확도와 크기는 서로 trade-off**
- **모델을 기기에 배포한 뒤 모델의 성능을 측정하고, 이를 바탕으로 모델을 다시 최적화하여 변환하고 기기에 배포**
