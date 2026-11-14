# 성인을 위한 필수 상식 가이드 프로그램 (Frontend)

기초 예절 및 사회 상식을 학습할 수 있는 데스크톱 애플리케이션의 프론트엔드 리포지토리입니다. 사지선다형 퀴즈와 카드 분류 게임의 사용자 인터페이스(UI)를 구현하고, 백엔드와 연동하여 사용자의 학습 이력을 시각적으로 제공합니다.

## 주요 화면 및 기능 (Core Features)
HomePanel(메인 대시보드) - (카테고리별 학습, 퀴즈 시작, 오답 노트, 학습 이력) 메뉴로 이동 가능.
CategoryPanel, ConceptStudyPanel(카테고리 선택 및 개념 학습) - 기초예절 및 사회상식의 카테고리별 학습 메뉴로 이동 가능. 학습 달성도 조회 가능.
HistoryPanel(학습 기록) - 점수 랭킹 메뉴로 이동 가능. 완료한 퀴즈 횟수, 평균 점수, 최고 점수, 퀴즈 응시 기록 조회 가능.
RankPanel(랭킹 시스템) - 전체 도전 횟수, 평균 점수, 최고 점수, 점수 랭킹 기록 조회 가능.
## 🛠 기술 스택 (Tech Stack)
* **Language:** Java
* **Design/Assets:** Figma

## 폴더 구조 (Directory Structure)
```text
src/
 ├── assets/       # 이미지, 아이콘, 폰트 등 정적 리소스 파일
 │   ├── icon_book.png
 │   ├── icon_play.png
 │   ├── icon_note.png
 │   ├── icon_chart.png
 │   ├── icon_manner.png
 │   └── icon_society.png
 ├ components/   # 버튼, 타이머, 카드 등 재사용 가능한 공통 UI 컴포넌트
 │   └── UIComponents.java
 ┣ views/        # 메인 화면, 퀴즈 화면, 결과 화면 등 전체 페이지 프레임
 │   ├── HomePanel.java
 │   ├── CategoryPanel.java
 │   ├── ConceptStudyPanel.java
 │   ├── HistoryPanel.java
 │   ├── RankPanel.java
 │   ├── NicknamePanel.java
 │   └── WrongNotePanel.java
 ┗ controller/   # 화면 간 전환 및 프론트엔드 내부 이벤트 처리
     ├── GUIMain.java
     └── DataMgr.java
