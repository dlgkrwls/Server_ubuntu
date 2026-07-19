<div align="center">

# 이학진 | Hakjin Lee

### Computer Vision · Deep Learning · Model Deployment

[![GitHub](https://img.shields.io/badge/GitHub-dlgkrwls-181717?style=flat-square&logo=github)](https://github.com/dlgkrwls)
[![Email](https://img.shields.io/badge/Email-Contact-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:202531048@sangmyung.kr)

</div>

---

## About Me

상명대학교 대학원에서 컴퓨터비전과 딥러닝을 연구하고 있습니다.

PyTorch 기반 모델 구현뿐만 아니라 데이터 전처리, 학습 및 평가,
정량 분석, Docker 기반 배포까지 전체 파이프라인을 경험했습니다.

현재 다음 분야의 Computer Vision / Machine Learning Engineer 직무를 준비하고 있습니다.

- Computer Vision
- Robust and Generalizable AI
- Image and Video Analysis
- Biometrics and Human-Centered AI
- Model Optimization and Deployment

---

## Tech Stack

### AI / Computer Vision

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white)

### Data / Experiment

![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=flat-square&logo=scipy&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-11557C?style=flat-square)

### Deployment / Development

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)
![VS Code](https://img.shields.io/badge/VS_Code-007ACC?style=flat-square&logo=visualstudiocode&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)

- Classification, Regression, Segmentation, Metric Learning
- Image, Video, 3D Pose and Time-Series Data Processing
- Custom Dataset and DataLoader Implementation
- Cross-Dataset Evaluation and Ablation Study
- Docker Image Build, Docker Hub Distribution and Ubuntu Deployment
- Research Experiment Design and Academic Writing

---

## Selected Projects

### 1. Docker-Based 3D Human Pose Video Analysis

> 비디오를 입력받아 프레임별 3D 관절 좌표를 추출하고 JSON으로 저장하는 분석 파이프라인

- 비디오 기반 3D human pose estimation 추론 파이프라인 구성
- 프레임별 16개 주요 관절의 3D 상대좌표 추출
- 입력 비디오와 분석 결과를 JSON 형식으로 연결
- 모델과 실행 환경을 Docker image로 패키징
- Docker Hub를 통한 이미지 배포
- Ubuntu 서버의 호스트 디렉터리와 컨테이너 간 volume mount 구성
- 컨테이너 종료 후에도 결과가 서버에 유지되도록 저장 구조 설계

```text
Input Video
    → Frame Processing
    → 3D Joint Estimation
    → Coordinate Normalization
    → JSON Generation
    → Host Server Storage
