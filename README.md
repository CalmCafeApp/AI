📖 개요

이 레포지토리는 카페 혼잡도 예측 시스템을 구현하기 위한 모든 핵심 요소를 포함하고 있습니다. 
CCTV 데이터를 기반으로 실시간 혼잡도를 모니터링하고, 과거 데이터를 활용하여 미래 혼잡도를 예측합니다.



🚀 주요 기능

1. 과거 데이터 기반 혼잡도 예측
CCTV 영상을 분석하여 움직임 및 좌석 데이터를 추출.
YOLOv8를 활용한 객체 탐지 결과를 CSV 파일로 저장.
Attention Mechanism, GRU, Seq2Seq, LSTM 모델을 비교 및 평가 후 Seq2Seq 모델로 최종 예측 수행.
예측 결과를 AWS S3에 저장하여 백엔드 API로 연동.

2. 실시간 혼잡도 모니터링
RTSP 프로토콜을 통해 실시간 CCTV 데이터를 스트리밍.
YOLOv8과 OpenCV를 활용해 실시간 객체 탐지 수행.
혼잡도를 퍼센트(%)로 계산하고, 한산, 보통, 혼잡으로 분류.
결과 데이터를 AWS S3에 저장 및 업데이트.

3. 자동화 및 확장성
Python Task Scheduler와 AWS EC2를 활용한 예측 작업 자동화 예정.
REST API를 통해 실시간 데이터 제공 예정.
백엔드 시스템과의 원활한 통합을 지원.

🎯 프로젝트 목표

실시간 및 정확한 혼잡도 데이터를 제공하여 사용자 만족도를 향상.
카페 관리자가 직원 배치 및 자원 관리를 최적화할 수 있도록 지원.
여러 카페에서 확장 가능하고 안정적인 AI 기반 시스템 구축.