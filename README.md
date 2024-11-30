# Pi-Golf 🏌️‍♂️

Pi-Golf는 Raspberry Pi와 Adafruit 1.3" Color TFT Bonnet을 사용하여 구현한 미니 골프 게임입니다.

## 주요 기능

- **지형 충돌과 바운스를 고려한 현실적인 골프 공 물리**
- **Perfect/Great/Cool로 평가되는 파워 게이지 시스템**
- **거리 추적 및 점수 시스템 (Par, Birdie, Eagle 등)**
- **TFT Bonnet의 조이스틱과 버튼을 이용한 직관적인 컨트롤**

---

## 하드웨어 요구사항

- Raspberry Pi 4 Model B
- Adafruit 1.3" Color TFT Bonnet for Raspberry Pi (240x240 TFT + Joystick)

## 소프트웨어 요구사항

```bash
sudo pip3 install adafruit-circuitpython-rgb-display
sudo apt-get install fonts-dejavu
```

---

## 디렉토리 구조

```
pi-golf/
├── src/
│   ├── __init__.py
│   ├── main.py
│   ├── Ball.py
│   ├── Hole.py
│   ├── Joystick.py
│   ├── PowerGauge.py
│   ├── Terrain.py
│   └── GameManager.py
└── README.md
```

---

## 컨트롤 방법

- **좌/우**: 샷 각도 조정
- **A 버튼**: 파워 게이지 시작/샷 실행
- **센터 버튼**: 게임 리셋

---

## 설치 방법

1. Raspberry Pi에서 SPI를 활성화합니다:
```bash
sudo raspi-config
# "Interface Options" -> "SPI" -> Enable
```

2. 이 저장소를 클론합니다:
```bash
git clone https://github.com/hwouu/pi-golf-ver3.git
cd pi-golf-ver3
```

3. 게임을 실행합니다:
```bash
python3 src/main.py
```

---

## 개발 배경

이 프로젝트는 임베디드 시스템 강의 프로젝트의 일환으로, 하드웨어와 소프트웨어 통합을 배우는 동시에 재미있는 게임 경험을 만드는 것을 목표로 합니다.

---

## 라이선스

이 프로젝트는 MIT 라이선스 하에 오픈 소스로 제공됩니다.


