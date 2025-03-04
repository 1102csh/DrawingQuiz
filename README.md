<h1 align="center">🎨 DrawingQuiz</h1>

<p align="center">
  <strong>Java로 제작한 소켓 통신을 활용한 스케치 퀴즈 게임</strong>
</p>

## 🚀 주요 기능

### 🎮 게임 플레이
- 최대 **4명**의 유저가 **게임에 참여** 가능합니다.
- 한 명의 유저가 그림을 그리며, 다른 유저들은 **채팅**을 통해 그 그림이 무엇인지 맞춥니다.
- **랜덤 그림 그리기 유저** : 매 라운드마다 한 명의 유저가 랜덤으로 그림을 그리게 됩니다.
- **실시간 그림 전송** : 그려지는 그림은 실시간으로 모든 유저에게 동일하게 보여집니다.
- **정답 맞추기** : 유저들이 채팅을 통해 정답을 맞추면 점수가 쌓입니다.

### 💾 유저 관리
- **MariaDB**를 사용하여 유저를 관리
- **회원가입 및 로그인 기능**

### 🎲 게임 라운드
- **15개 랜덤 단어**를 **DB에서 중복 없이 가져와** 각 라운드마다 그림 그리기 유저에게 제공됩니다.
- 각 라운드는 **15라운드**까지 진행되며, **맞춘 문제에 따라 점수**가 쌓입니다.
- **게임 종료 후 점수판**에서 유저의 점수를 확인할 수 있습니다.

### 🎶 오디오 효과
- **배경음악**과 **효과음**이 삽입되어 게임의 몰입감을 더해줍니다.

### 🖼️ GUI
- **JavaFX와 SceneBuilder**를 사용하여 깔끔하고 직관적인 **UI**를 제공합니다.

---

## 🛠️ 기술 스택

<p align="center">
  <img src="https://img.shields.io/badge/Java-007396?style=flat&logo=java&logoColor=white" alt="Java Badge" />
  <img src="https://img.shields.io/badge/JavaFX-2C2F3A?style=flat&logo=java&logoColor=white" alt="JavaFX Badge" />
  <img src="https://img.shields.io/badge/MariaDB-003545?style=flat&logo=mariadb&logoColor=white" alt="MariaDB Badge" />
  <img src="https://img.shields.io/badge/Sockets-808080?style=flat&logo=java&logoColor=white" alt="Sockets Badge" />
</p>

---

## 📌 프로젝트 흐름

1. **회원가입/로그인**: 유저는 먼저 **회원가입** 또는 **로그인**을 통해 게임에 접속합니다.
2. **게임 로비**: 로그인 후 게임 로비로 이동합니다. 최대 4명까지 접속할 수 있습니다.
3. **게임 진행**: 매 라운드마다 **그림 그리기 유저**가 랜덤으로 선택되며, 그 유저는 제시된 단어 중 하나를 그림으로 그립니다.
4. **정답 맞추기**: 나머지 유저는 **채팅**을 통해 정답을 맞추며 점수를 얻습니다.
5. **게임 종료 후**: 15라운드가 끝나면 점수판을 통해 유저들의 점수를 확인하고, **다음 게임**을 시작할 수 있습니다.

---
