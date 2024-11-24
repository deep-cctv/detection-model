# detection-model

deep-cctv 에서 폭력을 감지하기 위한 모델

## 개요

kaggle 의 데이터로 MobileNetV2 모델을 학습시킨다.

- [notbook 참고](mobilenetv2-model.ipynb)

실행 결과 생성된 모델 model.h5를 cctv-server 에서 사용한다.

## 실행

```bash
pip install -r requirements.txt
```

`mobilenetv2-model.py` 실행

### 실행 중 문제해결

#### `pip install -r requirements.txt` 실행 중 에러 발생 시

- python 버전을 3.11 을 사용한다.
- `tensorflow-io-gcs-filesystem` 를 제외하고 설치한다. (주석처리)
- 맥 또는 리눅스 환경에서 실행한다.
