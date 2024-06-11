# 설치

## 가상환경 셋팅

```bash
conda create -n teachable_ml_fastapi
conda activate teachable_ml_fastapi
```

## 패키지 설치

```bash
pip install -r requirements.txt
```

## FastAPI 실행

```bash
uvicorn predict:app --reload
```

## 테스트 FastAPI

서버가 실행되면, 브라우저에서 `http://127.0.0.1:8000/docs`로 이동하여 API 문서를 확인할 수 있습니다.

## 사용 방법

1. `/predict/` 엔드포인트에 이미지를 업로드하여 예측 결과를 얻을 수 있습니다.
2. 예측 결과는 JSON 형식으로 반환되며, 클래스 이름과 신뢰도 점수를 포함합니다.

## 코드 설명

- `predict.py` 파일은 FastAPI 애플리케이션을 정의합니다.
- Keras 모델과 클래스 레이블을 로드합니다.
- `/predict/` 엔드포인트는 이미지를 입력받아 예측 결과를 반환합니다.

## 모델은

강호동 김희선 송혜교 원빈 유재석
의 얼굴로 이름을 찾는 모델 샘플입니다.
