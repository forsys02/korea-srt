# 🚄 Korea SRT (Subtitle Translation & Media Agent)

[![Python Version](https://img.shields.io/badge/python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![AI Engine](https://img.shields.io/badge/AI-Gemini--Core-orange?logo=google-gemini&logoColor=white)](https://deepmind.google/technologies/gemini/)
[![UI Style](https://img.shields.io/badge/UI-TUI%20Console-green?logo=gnuprivacyguard&logoColor=white)](https://en.wikipedia.org/wiki/Text-based_user_interface)
[![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://opensource.org/licenses/MIT)

> **Gemini AI 기반의 고정밀 SRT 자막 번역 및 미디어 다운로드/재생 통합 관제 TUI 에이전트**  
> 복잡한 자막 싱크 보정, 다국어 번역, 유튜브 미디어 다운로드, 그리고 텔레그램 봇을 통한 PC 원격 제어까지 단 하나의 스크립트로 완벽하게 처리해냥! 🐾

---

## ✨ 핵심 기능 (Key Features)

### 🧠 1. Gemini AI 기반 스마트 자막 번역 & 싱크 보정
* **초정밀 자막 번역**: Google Gemini API를 활용하여 맥락을 파악하고 자연스러운 구어체 번역을 수행합니다.
* **OTP(One-to-One Time) 싱크 엔진**: 번역 시 타임라인이나 시간축이 어긋나지 않도록 원본 시간 데이터를 철저하게 보존합니다.
* **무삭제 번역 엔진**: 어색하게 생략되는 구간 없이 원문의 뉘앙스를 고스란히 자막에 살려냅니다.

### 📥 2. 유튜브/미디어 다운로드 & 메타데이터 자동 추출
* **최적화 다운로드**: 최고 화질/음질의 포맷을 지능적으로 선별하여 안정적으로 미디어를 다운로드합니다.
* **자동 챕터 매핑**: 다운로드한 동영상에 메타데이터 및 유튜브 챕터를 자동으로 주입해 줍니다.

### 🐕 3. 텔레그램 봇 기반 원격 관제 (Binu Watchdog)
* **백그라운드 감시**: 메인 프로세스가 꺼져 있어도 독립적인 워치독(`watchdog.py`) 프로세스가 텔레그램 메시지를 수신하여 원격으로 메인 앱을 재가동하거나 종료할 수 있습니다.
* **PC 원격 제어**: 텔레그램 채팅방에서 간편한 인라인 버튼 터치로 PC 절전, 재부팅, 볼륨 조절, 재생 제어가 가능합니다.

### ⌨️ 4. 강력하고 직관적인 TUI(Text User Interface) 및 단축키 마법사
* **키보드 친화적 설계**: 마우스 없이 방향키와 단축키(예: `q`, `xx` 등)만으로 모든 미디어 탐색, 자막 번역, 환경 설정을 광속으로 처리합니다.
* **지능형 파일 탐색**: 휴지통 즉시 정렬, 폴더별 개별 정렬 정보 기억, 다중 선택 모드를 지원합니다.

---

## 🚀 시작하기 (Quick Start)

### 📋 요구 사항
* **OS**: Windows 환경을 완벽하게 지원합니다. (UAC 관리자 승격 및 윈도우 단축키, 네이티브 Event 신호 연동)
* **Python**: 3.8 버전 이상이 필요합니다.

### ⚙️ 설치 및 실행 방법

별도의 복잡한 패키지 설치 과정이 필요하지 않습니다. 실행 시 누락된 필수 라이브러리를 자동으로 감지하고 `pip`로 알아서 설치해 줍니다! 👍

1. 본 저장소에서 **korea.srt.py** 단일 파일을 다운로드합니다.
2. 터미널(Command Prompt 또는 PowerShell)을 열고 아래 명령어로 스크립트를 가동합니다:
   ```bash
   python korea.srt.py
   ```

---

## 🔧 설정 및 사용 가이드

### 1. 첫 실행 및 UAC 권한 승격
* 스텔스 엔진 구동 및 단축키 연동 등의 원활한 시스템 제어를 위해 실행 시 **UAC 관리자 권한 승격 창**이 나타날 수 있습니다. 승인하면 정상 구동됩니다.

### 2. 텔레그램 봇 및 API 설정
* TUI 메뉴 내의 **환경 설정** 메뉴로 진입하여 Gemini API Key, GitHub ID, Telegram Token 및 Chat ID를 입력할 수 있습니다.
* 모든 설정 정보는 로컬에 `settings.json` 파일로 암호화 및 안전하게 저장됩니다.

### 3. 워치독(Watchdog) 구동
* 메인 메뉴의 **Watchdog 관리** 메뉴에서 `와치독 설치/갱신`을 선택하면 실행 환경의 경로에 맞춰 백그라운드에서 상시 감시하는 `watchdog.py`가 자동으로 안전하게 생성됩니다.

---

## 📝 라이선스 (License)
이 프로젝트는 [MIT License](https://opensource.org/licenses/MIT)에 따라 배포됩니다.
자유롭게 수정 및 배포가 가능하나 개인 정보 유출이나 오용에 주의해 주시기 바랍니다.

---

> Created by **Binu** 💖  
> 버그 제보나 아이디어 제안은 언제나 환영이다냥! 🐱🐾
