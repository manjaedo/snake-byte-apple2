# 🐍 APPLE ][ - SNAKE BYTE (1982 Sirius Software)

1982년 **Sirius Software**(Chuck Sommerville 제작)의 Apple II용 8비트 고전 명작 게임 **스낵바이트(Snake Byte)**를 웹 표준(HTML5 Canvas + Web Audio API)으로 재현한 프로젝트입니다.

## ✨ 주요 특징
- **Disk II 플로피 디스크 부팅 인트로:**
  - Apple II 전원 비프음(`1000Hz`) 및 Disk II 트랙 0 헤드 캘리브레이션 구동음 재현
  - DOS 3.3 `CATALOG` → `BRUN SNAKE.BYTE` 실행 및 Apple II Hi-Res(`$2000~$3FFF`) 인터리브 메모리 블라인드 로딩 효과
- **3가지 CRT 모니터 모드 (`M` 키 전환):**
  - `🌈 8-BIT COLOR`: Apple II Hi-Res 6색 아티팩트 컬러
  - `🟠 주홍색 (AMBER)`: 호박색 단색 CRT 모니터
  - `🟢 초록색 (GREEN)`: Apple Monitor II/III P31 녹색 단색 CRT 모니터
- **4단계 통합 난이도 (자두 개수 0~2개 + 이동 속도 조합):**
  - `[0] EASY`: 자두 0개 • 느린 속도 (`215ms`)
  - `[1] NORMAL`: 자두 1개 • 보통 속도 (`170ms`, 기본값)
  - `[2] HARD`: 자두 2개 • 빠른 속도 (`135ms`)
  - `[3] EXPERT`: 자두 2개 • 초고속 (`100ms`)
- **오리지널 게임 규칙 & 28개 전체 스테이지:**
  - 각 레벨에서 사과 10개를 먹으면 상단 중앙의 탈출문(Exit Gate) 개방
  - 좌우 벽면을 타고 올라오는 타임아웃 바(시간 초과 시 페널티 사과 추가)
  - **4-KEY**(방향키/WASD) 조작 및 오리지널 **2-KEY**(진행 방향 기준 좌/우 90° 회전) 모드 지원

## 💻 다른 컴퓨터에서 이어서 작업하기
```bash
git clone https://github.com/manjaedo/snake-byte-apple2.git
cd snake-byte-apple2
```
클론 받은 폴더를 Antigravity의 활성 워크스페이스(Active Workspace)로 열거나 `index.html` 파일을 브라우저에서 바로 실행하면 됩니다.
