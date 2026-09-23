# 실행 조건

2024년 기말 보고서에 수록한 주행 코드의 빈 줄과 서식을 정리해 `src/drive.py`로 복원했습니다. 당시 Raspberry Pi 차량·카메라·GPIO 배선과 다음 자료가 필요합니다.

| 별도 자료 | 용도 |
|---|---|
| 수업용 `SDcar` 라이브러리 | 모터 제어 |
| `lane_navigation_*.h5` | 학습한 방향 분류 모델 |
| `frozen_inference_graph.pb` | SSD MobileNet v2 가중치 |
| `ssd_mobilenet_v2_coco_2018_03_29.pbtxt` | 객체 인식 모델 설정 |
| `object_detection_classes_coco.txt` | 객체 이름 목록 |

코드의 모델 경로와 GPIO 배선을 환경에 맞춘 뒤 `src`에서 실행합니다. `requirements.txt`는 import 기준 목록이며 당시 환경의 버전 잠금 파일은 아닙니다.

코드 문법 검사를 진행해 오류가 없음을 확인했습니다. 차량에서 다시 실행하거나 주행 성능을 재측정하지는 않았습니다.
