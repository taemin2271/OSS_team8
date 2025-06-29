<details>
<summary>Korean README</summary>

# 🏰  2D 타워 디펜스 게임(Korean)

## ✨ 개요

Pygame으로 제작된 2D 타워 디펜스 게임입니다. 전략적으로 타워를 배치하여 몰려오는 적을 막고, 최고의 방어 전략을 세워보세요!

## 🎮 주요 기능

-   **다양한 타워**:
    -   기본 타워, 스나이퍼 타워, 슬로우 타워 등 개성 넘치는 타워들을 건설하세요.
    -   각 타워는 고유한 능력과 업그레이드 옵션을 제공합니다.
-   **전략적인 웨이브 시스템**:
    -   웨이브 매니저를 통해 난이도가 점진적으로 상승하는 적들을 상대하세요.
    -   각 웨이브를 분석하고, 다음 웨이브에 대비하세요.
-   **직관적인 UI**:
    -   상점, 골드, 다음 웨이브, 일시정지 버튼 등 편리한 UI를 통해 게임을 컨트롤하세요.
    -   필요한 정보를 한눈에 확인하고, 효율적인 전략을 구상하세요.
-   **다양한 게임 씬**:
    -   메인 메뉴, 게임 플레이, 일시정지, 게임 오버, 클리어 씬을 통해 게임의 흐름을 느껴보세요.
    -   각 씬은 몰입감 있는 경험을 제공합니다.
-   **개성 넘치는 적 유닛**:
    -   각기 다른 체력과 능력을 가진 적들을 막아내세요.
    -   적들의 특성을 파악하고, 효과적인 타워 조합을 구성하세요.
-   **전략적인 타워 설치 제한**:
    -   경로 근처나 이미 타워가 설치된 위치에는 타워를 설치할 수 없습니다.
    -   지형을 활용하고, 최적의 방어 라인을 구축하세요.

## 🕹️ 게임 방법

1.  **타워 선택**: 상점에서 원하는 타워를 선택하세요. 각 타워는 고유한 가격과 능력을 가지고 있습니다.
2.  **타워 설치**: 맵의 전략적인 위치에 타워를 설치하세요. 타워는 골드를 소모하며, 위치 선정이 중요합니다.
3.  **웨이브 시작**: "Next Wave" 버튼을 클릭하여 다음 웨이브를 시작하세요. 웨이브마다 더 강력한 적들이 등장합니다.
4.  **적 방어**: 타워를 이용하여 몰려오는 적들을 막으세요. 타워의 공격 범위와 능력을 활용하여 효율적으로 방어하세요.
5.  **골드 획득**: 적을 처치하면 골드를 획득합니다. 획득한 골드로 더 강력한 타워를 건설하세요.
6.  **게임 승리 조건**: 모든 웨이브를 클리어하면 게임에서 승리합니다. 최고의 전략가가 되어보세요!
7.  **게임 패배 조건**: 적이 기지를 특정 횟수 이상 통과하면 게임에서 패배합니다. 방어선을 굳건히 지키세요!

## ⚙️ 조작 방법

-   **마우스**:
    -   타워 선택 및 설치
    -   UI 버튼 클릭 (상점, 다음 웨이브, 일시정지 등)
-   **키보드**:
    -   `P`: 일시정지 (Pause)

## 🧩 게임 구성 요소

### 1. `main.py`

-   게임의 핵심 로직을 담당합니다.
-   Pygame 초기화, 창 설정, 게임 루프, 이벤트 처리 등을 관리합니다.
-   게임 상태 (메뉴, 플레이, 일시정지, 게임 오버, 클리어)를 제어합니다.

### 2. `enemies.py`

-   `Enemy` 클래스를 정의합니다.
-   적의 위치, 경로, 체력, 이동 속도, 폭발 애니메이션 등을 관리합니다.
-   다양한 적들의 행동 패턴을 구현합니다.

### 3. `tower.py`

-   `Tower` 클래스 (기본 타워, 스나이퍼 타워, 슬로우 타워) 및 `Bullet` 클래스를 정의합니다.
-   타워의 공격 범위, 데미지, 쿨다운 등을 설정합니다.
-   총알의 이동 및 적중 로직을 처리합니다.

### 4. `wave_manager.py`

-   `WaveManager` 클래스를 정의합니다.
-   웨이브 생성, 적 스폰, 웨이브 진행 상태 등을 관리합니다.
-   웨이브의 난이도와 적의 구성을 제어합니다.

### 5. `UI.py`

-   `Button`, `TextDisplay`, `Shop` 클래스를 정의합니다.
-   게임 내 UI 요소 (버튼, 텍스트, 상점)를 생성하고 관리합니다.
-   사용자 인터페이스를 통해 게임과 상호작용합니다.

### 6. `Scene.py`

-   `MainMenu`, `Pause`, `GameOver`, `ClearScene` 클래스를 정의합니다.
-   각 씬의 화면을 구성하고, 이벤트 처리 로직을 담당합니다.
-   게임의 각 단계를 시각적으로 표현합니다.

## 🛠️ 설치 및 실행 방법

1.  **Pygame 설치**:

    ```bash
    pip install pygame
    ```

2.  **게임 파일 다운로드**:

    -   GitHub 저장소에서 게임 파일을 다운로드합니다.

3.  **게임 실행**:

    ```bash
    python main.py
    ```

## 📝 추가 개선 사항 (TODO)

-   더욱 다양한 종류의 타워 및 적 유닛 추가
-   타워 업그레이드 기능 추가
-   더욱 정교한 맵 디자인 및 다양한 맵 추가
-   사운드 효과 및 배경 음악 추가
-   난이도 설정 기능 추가
-   튜토리얼 모드 추가

## 🧑‍💻 팀원

-   Team8

## 📜 라이선스

MIT License

</details>

<details>
<summary> English README</summary>

# 🏰 2D Tower Defense Game (English)

## ✨ Overview  
This is a 2D Tower Defense game built with Pygame. Strategically place towers to block incoming enemies and build the ultimate defense strategy!

## 🎮 Key Features  
- **Various Towers**: Build towers like Basic, Sniper, and Slow Tower with unique abilities.  
- **Strategic Wave System**: Use the Wave Manager to face stronger enemies over time.  
- **Intuitive UI**: Includes shop, gold counter, next wave button, and pause button.  
- **Multiple Scenes**: Includes Main Menu, Gameplay, Pause, Game Over, and Clear.  
- **Unique Enemy Units**: Defend against enemies with different health and abilities.  
- **Strategic Placement Limits**: Towers cannot be placed near paths or on existing towers.

## 🕹️ How to Play  
1. Select a tower → 2. Place the tower → 3. Start the wave → 4. Defend → 5. Earn gold  
- Win by clearing all waves  
- Lose if too many enemies reach the base

## ⚙️ Controls  
- Mouse: Place towers, click UI buttons  
- Keyboard: `P` for pause

## 🧩 Game Components  
- `main.py`: Game loop and state management  
- `enemies.py`: Enemy unit classes  
- `tower.py`: Tower and bullet classes  
- `wave_manager.py`: Manages enemy waves  
- `UI.py`: Buttons, shop, and text display  
- `Scene.py`: Game scene layouts

## 🛠️ Installation & Execution  
```bash
pip install pygame
python main.py
```

## 📝 TODO: Future Improvements
- Add more tower and enemy types  
- Implement upgrade system  
- Add maps and background music  
- Difficulty settings and tutorial mode  

## 🧑‍💻 Team
Team8

## 📜 License
MIT License

</details>
