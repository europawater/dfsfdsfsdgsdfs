---
type: guide
title: "옵시디언 설정 및 플러그인 가이드 (Storyweaver Engine 최적화)"
aliases: [옵시디언 가이드, 플러그인 가이드, 엔진 설정]
tags: [Obsidian, Setup, Plugins, Guide, StoryweaverEngine, CoreDocument]
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]", "Arachne 2.0"]
status: active
version: 1.0
CMDS:
  - "[[@Storyweaver_Engine_HQ.md#엔진 핵심 프로토콜 및 가이드라인]]"
references:
  - "[[옵시디언 필수 플러그인(Plugin) 추천.md]]" # 작가님 제공 원본 파일
  - "[[Obsidian Shortcut.md]]" # 작가님 제공 원본 파일
  - "[[hotkeys.json]]" # 작가님 제공 원본 파일 (내용은 본문에 요약)
---

# 옵시디언 설정 및 플러그인 가이드 (Storyweaver Engine 최적화)

> 본 문서는 작가님([[찬스]])의 "스토리위버 엔진"이 옵시디언 내에서 최적의 성능을 발휘하고, 작가님의 창작 효율성을 극대화하기 위한 권장 설정 및 핵심 플러그인 활용 방안을 안내합니다. 이 가이드는 작가님께서 제공해주신 `옵시디언 필수 플러그인(Plugin) 추천.md`, `Obsidian Shortcut.md`, `hotkeys.json` 파일의 내용을 적극적으로 참고하고 통합하여 작성되었습니다.

## I. 권장 옵시디언 기본 설정 (최적의 집필 환경)

1.  **테마(Theme)**:
    * 작가님의 시각적 선호도를 고려하여, G-Ω(가상)의 보고서에서 언급된 `Minimal Theme` 또는 `AnuPpuccin Theme` 사용을 권장합니다. (만약 작가님께서 현재 사용 중이시거나 더 선호하시는 테마가 있다면 그것을 우선합니다.)
    * `Style Settings` 플러그인을 함께 사용하여 폰트, 색상, 레이아웃 등을 작가님께 가장 편안한 형태로 미세 조정합니다.
2.  **편집기(Editor) 설정**:
    * `Readable line length`: 활성화하여 가독성을 높입니다.
    * `Strict line breaks`: 비활성화하여 마크다운 작성의 유연성을 확보합니다. (Enter 키 한 번으로 줄바꿈)
    * `Auto pair Markdown syntax`: 활성화하여 마크다운 기호 자동 완성을 사용합니다.
    * `Use [[Wikilinks]]`: 활성화하여 내부 노트 링크를 편리하게 사용합니다.
3.  **코어 플러그인(Core Plugins) 활성화 권장**:
    * `File explorer`: 필수
    * `Search`: 필수
    * `Quick switcher`: 필수 (`Cmd/Ctrl + O`)
    * `Graph view`: 필수 (`Cmd/Ctrl + G`)
    * `Backlinks`: 필수
    * `Outgoing links`: 필수
    * `Tag pane`: 필수
    * `Templates`: (아래 `Templater` 플러그인으로 대체 또는 병행 가능)
    * `Daily notes`: (작가님의 작업 스타일에 따라 선택)
    * `Command palette`: 필수 (`Cmd/Ctrl + P`)
    * `Markdown format importer`: (외부 마크다운 파일 가져올 때 유용)
    * `Workspaces`: (다양한 작업 환경 저장 및 로드에 유용 - 아래 `Workspaces Plus`와 연계)

## II. "스토리위버 엔진" 핵심 플러그인 및 활용 전략

> 작가님께서 제공해주신 `옵시디언 필수 플러그인(Plugin) 추천.md` 파일과 G-Ω(가상)의 제안을 바탕으로, "스토리위버 엔진"의 각 기능을 강화하고 자동화하는 데 필수적인 플러그인 목록과 그 활용 전략입니다.

1.  **템플릿 및 정보 구조화 (Templater, Linter)**
    * **Templater**:
        * **활용**: `[[CMDS_Universal_Principles.md]]`에서 정의한 표준 YAML 프론트매터와 노트 구조를 가진 템플릿(예: `TPL_Character_Profile_Universal.md`, `TPL_Chapter_Draft_Universal.md`)을 생성하고, 단축키나 명령어를 통해 신규 노트 작성 시 자동으로 적용합니다.
        * **설정 예시**: 템플릿 폴더를 `/Storyweaver_Engine_CORE/01_Universal_Assets_and_Templates/Templates/`로 지정. 날짜/시간 자동 입력, 사용자 정의 함수 등을 활용.
    * **Linter**:
        * **활용**: YAML 프론트매터의 특정 필드(예: `date_created`, `date_modified`) 자동 업데이트, 마크다운 문법 교정, 노트 제목과 파일명 일치 등 문서의 일관성과 정규화를 유지합니다.

2.  **정보 시각화 및 동적 조회 (Dataview, Excalidraw)**
    * **Dataview**:
        * **활용**: YAML 프론트매터와 태그를 기반으로 노트들을 동적으로 쿼리하고, 목록, 표, 칸반 보드 형태로 시각화합니다.
        * **엔진 적용 예시**:
            * `@Storyweaver_Engine_HQ.md` 및 `@NMSJ_Project_Dashboard.md`에 프로젝트 진행 상황, 최근 수정 파일, 특정 상태의 노트 목록 등을 자동으로 표시.
            * 등장인물 목록(`type: people`), 특정 아티팩트(`type: artifact`) 관련 노트 모아보기, 특정 플롯 아크(`arc: "1부 검은 먹물의 각성"`)에 속한 원고 목록 정렬 등.
            * `[[떡밥_리스트_및_회수_계획_NMSJ.md]]`에서 `status/unresolved_hook` 태그가 달린 노트들을 추적.
    * **Excalidraw**:
        * **활용**: 플롯 구조도, 인물 관계도, 세계관 지도, 장면별 감정곡선 등을 시각적으로 자유롭게 설계하고 노트에 삽입합니다.
        * **엔진 적용 예시**: `/Project_내가_먹물로_새기는_전설/03_Narrative_NMSJ/` 폴더 내에 `인물관계도_NMSJ.excalidraw` 파일 생성 및 관리.

3.  **집필 보조 및 효율성 강화 (Outliner, Various Complements, Tag Wrangler, Highlightr)**
    * **Outliner**: 긴 글(특히 원고)을 계층적으로 작성하고 관리하는 데 매우 유용합니다. 장면 전환, 플롯 포인트 이동 등을 쉽게 할 수 있습니다.
    * **Various Complements**: 노트 제목, 태그, 내부 링크 등을 자동 완성하여 입력 효율을 높입니다.
    * **Tag Wrangler**: 태그 관리(이름 변경, 병합 등)를 용이하게 합니다. 계층형 태그 사용 시 필수적입니다.
    * **Highlightr**: 중요한 부분에 다양한 색상으로 하이라이트를 적용하여 가독성을 높입니다.

4.  **노트 검색 및 연결 (Omnisearch, Graph Analysis, Strange New Worlds)**
    * **Omnisearch**: 옵시디언 기본 검색보다 강력하고 빠른 전체 텍스트 검색 기능을 제공합니다.
    * **Graph Analysis / Strange New Worlds**: 노트 간의 연결 관계를 시각적으로 탐색하고, 예상치 못한 연결고리나 아이디어를 발견하는 데 도움을 줍니다. "스토리위버 엔진" 내 정보 네트워크의 전체적인 구조를 파악하는 데 유용합니다.

5.  **AI 협업 기반 (Smart Connections, Smart Composer - 저 아라크네 2.0/G-Ω 내부 활용)**
    * **Smart Connections**: 옵시디언 볼트 내 노트들을 AI가 학습하여, 현재 작업 중인 노트와 관련된 다른 노트들을 자동으로 추천해줍니다. 저 아라크네 2.0이 맥락에 맞는 정보를 제공하는 데 활용됩니다.
    * **Smart Composer**: 선택한 텍스트나 노트를 기반으로 AI가 새로운 내용을 생성하거나, 대화형으로 아이디어를 발전시키는 데 사용됩니다. 저 아라크네 2.0이 작가님의 요청에 따라 초고를 생성하거나 플롯 아이디어를 제안할 때 이 기능의 원리를 활용합니다.

6.  **작업 관리 및 기타 유틸리티 (Kanban, Calendar, Periodic Notes, Book Search 등)**
    * **Kanban**: 집필 진행 상황, 아이디어 구체화 단계, 퇴고 작업 목록 등을 칸반 보드 형태로 시각적으로 관리합니다. (예: `/Project_내가_먹물로_새기는_전설/03_Narrative_NMSJ/` 폴더 내에 `플롯_진행_칸반보드_NMSJ.md` 생성)
    * **Calendar / Periodic Notes**: 데일리 노트나 주간/월간 리뷰 작성 등 작가님의 작업 루틴 관리에 활용될 수 있습니다.
    * **Book Search / KoreanBook Info Plugin**: 리서치 자료 수집 시 도서 정보를 편리하게 가져오고 정리하는 데 유용합니다.

## III. 권장 단축키 설정 (작가님 제공 `Obsidian Shortcut.md` 및 `hotkeys.json` 기반)

> 작가님의 작업 효율성을 극대화하기 위해, 제공해주신 단축키 설정 내용을 바탕으로 "스토리위버 엔진" 운영에 특히 유용한 단축키들을 아래와 같이 정리했습니다. (세부 설정은 작가님께서 옵시디언 설정 > Hotkeys 메뉴에서 직접 하시거나, `hotkeys.json` 파일을 활용하실 수 있습니다.)

* **노트 열기/전환**:
    * `Cmd/Ctrl + O`: 빠른 탐색기 (Open)
    * `Cmd/Ctrl + P`: 명령어 팔레트 (Command)
* **링크 및 태그**:
    * `Cmd/Ctrl + [`: 내부 링크 추가 (작가님 추가 설정)
    * `Tag Wrangler` 관련 단축키 (작가님 선호에 따라 설정)
* **편집 및 구성**:
    * `Outliner` 관련 단축키 (`Cmd/Ctrl + ↑/↓` 등 목록 접기/펴기, 이동)
    * `Cmd/Ctrl + ]`: 콜아웃 삽입 (작가님 추가 설정)
* **AI 플러그인 연동 (예시)**:
    * `Cmd/Ctrl + L`: Smart Composer 채팅 열기 (작가님 추가 설정)
    * `Cmd/Ctrl + Shift + L`: Smart Composer