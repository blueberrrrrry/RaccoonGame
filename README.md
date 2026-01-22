# 🦝 RaccoonGame - AI 기반 제스처 인식 3D 게임

손과 얼굴 인식을 활용한 인터랙티브 3D 러닝 게임입니다.

## 🎮 게임 소개

TensorFlow.js와 MediaPipe를 활용하여 실시간으로 손동작과 얼굴 기울기를 인식하고, 이를 통해 3D 캐릭터를 조작하는 게임입니다. 제스처에 따라 다양한 동물로 변신하며 장애물을 피해 동물원을 탈출하세요!

## ✨ 주요 기능

- **실시간 AI 인식**: TensorFlow.js와 MediaPipe를 활용한 손동작 및 얼굴 인식
- **3D 게임 환경**: Three.js 기반 3D 그래픽스
- **동적 캐릭터 변신**: 제스처에 따른 실시간 3D 모델 교체
- **적응형 난이도**: 라운드별 속도 증가 및 장애물 생성 패턴 조절
- **멀티미디어 통합**: 배경음악, 효과음, 3D 모델 애니메이션

## 🎯 게임 방법

### 기본 조작
- **좌/우 이동**: 얼굴을 좌우로 기울이기
- **변신**: 손동작으로 동물 변신 (좌우 반전 가능)

### 변신 제스처
- 👍 **코끼리**: 나무 부수기
- ✌ **토끼**: 슈퍼 점프로 장애물 뛰어넘기
- ✊ **뱀**: 독으로 바위 녹이기
- 👆 (뒤집기) **호랑이**: 포효로 사람 도망시키기

## 🚀 배포된 게임 플레이

GitHub Pages를 통해 배포된 게임을 플레이할 수 있습니다:
**https://blueberrrrrry.github.io/RaccoonGame/**

## 🛠️ 기술 스택

- **프론트엔드**: HTML5, CSS3, JavaScript (ES6+)
- **3D 엔진**: Three.js
- **AI 처리**: TensorFlow.js, MediaPipe
- **모델 형식**: GLTF/GLB

## 📦 로컬 실행 방법

1. 저장소 클론
```bash
git clone https://github.com/blueberrrrrry/RaccoonGame.git
cd RaccoonGame
```

2. 웹 서버 실행 (예: Python)
```bash
# Python 3
python -m http.server 8000

# 또는 Node.js (http-server)
npx http-server
```

3. 브라우저에서 접속
```
http://localhost:8000/index.html
```

**주의**: 웹캠 권한이 필요하며, HTTPS 환경 또는 localhost에서만 작동합니다.

## 📝 프로젝트 구조

```
RaccoonGame/
├── animal/              # 동물 3D 모델
├── background/          # 배경 3D 모델
├── obstacle/            # 장애물 3D 모델
├── image/               # 이미지 리소스
├── music/               # 오디오 파일
├── *.js                 # 게임 로직 모듈
├── start.html           # 게임 메인 페이지
├── index.html           # 시작 화면
└── ending.html          # 엔딩 화면
```

## 🔧 개발

### 주요 모듈
- `hand-face-recognition.js`: AI 기반 제스처 및 얼굴 인식
- `main.js`: 게임 초기화 및 시스템 통합
- `scene-setup.js`: 3D 환경 구성
- `model-loader.js`: 3D 모델 동적 로딩
- `game-state.js`: 게임 상태 관리
- `collision-system.js`: 물리 충돌 감지
- `animation-loop.js`: 게임 루프 제어

## 📄 라이선스

이 프로젝트는 교육 목적으로 개발되었습니다.

## 👤 개발자

blueberrrrrry

---

**게임을 즐기시고, 문제가 있으면 이슈를 등록해주세요!** 🎉
