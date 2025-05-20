---
type: portal
title: "내가 먹물로 새기는 전설 - 프로젝트 대시보드"
aliases: [NMSJ_Dashboard, 내가 먹물로 새기는 전설 대시보드]
tags: [project_dashboard, NMSJ, web_novel]
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: [[찬스]]
project_id: NMSJ
status: Phase2_InitialDataInput # 또는 Dataview로 관리되는 상세 상태
current_arc: 1부 검은 먹물의 각성
next_milestone: 프로젝트 초기 데이터 입력 완료 및 3화 집필 착수
version: 1.1 # YAML 구조 변경 반영
CMDS: 
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Storyweaver_Engine_HQ#현재_진행_중인_프로젝트]]"
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/CMDS_Universal_Principles#프로젝트_관리]]"
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Author_Style_Guide_Main#작품별_스타일_가이드]]"

# === Arachne 2.0 협업 강화 필드 ===
last_session_summary: "YAML 프론트매터 관리 지침 수립 및 적용 방안 논의 완료. 주요 문서 및 템플릿 업데이트 예정."
next_action_required: "제안된 YAML 구조를 템플릿 및 주요 NMSJ 문서에 적용 시작. (1차: 대시보드, 원고, 캐릭터, 아티팩트)"
arachne_feedback_status: "approved" # 작가님의 이번 지침에 대한 상태

# === 현재 작업 컨텍스트 (Arachne 2.0용) ===
current_task_context:
  task_id: "NMSJ_YAML_Update_Phase1"
  objective: "NMSJ 프로젝트의 핵심 문서 및 템플릿에 새로운 YAML 프론트매터 구조를 적용하여 AI 협업 효율성 증대."
  required_documents:
    - "[[Author_Projects/Project_내가_먹물로_새기는_전설/@NMSJ_Project_Dashboard.md]]"
    - "[[📂 Storyweaver_Engine_CORE/01_Universal_Assets_and_Templates/Templates/TPL_Chapter_Draft_Universal.md]]"
    - "[[Author_Projects/Project_내가_먹물로_새기는_전설/04_Manuscript_NMSJ/EP01_NMSJ/1화_검은재앙_피로쓰다_NMSJ.md]]"
    - "[[Author_Projects/Project_내가_먹물로_새기는_전설/02_Lore_NMSJ/Characters_NMSJ/이도윤_주인공_NMSJ.md]]"
    # (기타 관련 문서들...)
  key_characters_in_focus: [] # 이번 작업에서 특별히 집중할 캐릭터 (필요시 명시)
  key_settings_in_focus: [] # 이번 작업에서 특별히 집중할 설정 (필요시 명시)
  critical_plot_points_to_resolve_or_introduce: [] # 플롯 관련 작업 시 명시
  continuity_checkpoints: # 연속성 확인이 필요한 사항 (필요시 명시)
    - "새로운 YAML 필드가 기존 CMDS 원칙 및 옵시디언 활용법과 충돌하지 않는지 확인"
---

# 🖋️ 내가 먹물로 새기는 전설 - 프로젝트 대시보드

> **"2025년 서울, 사채 빚에 시달리던 미술품 복원가 이도윤. 정체불명의 고대 먹 '삼한비록지묵'과 강제 계약 후, 잊혀진 역사의 기록과 힘을 얻어 거대한 음모에 맞선다!"**
>
> 이곳은 "내가 먹물로 새기는 전설" 프로젝트의 모든 정보로 연결되는 중앙 허브이자, 작가님([[찬스]])과 저 아라크네 2.0의 협업 지휘소입니다.

---

## 🎯 프로젝트 목표 및 현황 (Project Goals & Status)

- **최종 목표**: 문피아 1페이지 점령 및 200화+ 장기 연재
- **현재 상태**: `$=dv.current().status`
- **다음 마일스톤**: `$=dv.current().next_milestone`
- **전체 진행도 (개념적)**: (칸반 보드 링크 또는 주요 아크 완료도 표시 - 추후 설정)
- **핵심 가이드라인**:
    - **문체**: `[[Author_Style_Guide_Main]]` (절대 준수!)
    - **구조 참조**: `[[Webnovel_Success_Patterns_General]]` (옵시디언 내 `RP75_Guide.txt` 분석 노트 링크)

---

## 📖 작품 기본 정보 및 기획 (Project Brief & Genesis Chamber)

- **[[작품_기본_정보_및_로그라인_NMSJ|NMSJ 로그라인]]** (상세 내용)
- **[[📂 00_프로젝트_개요_NMSJ/문체_고정_가이드라인_NMSJ.md|프로젝트 특화 문체 노트 (필요시)]]**
- **[[📂 01_Genesis_NMSJ/핵심_아이디어_및_키워드_맵_NMSJ.md|핵심 아이디어 및 키워드 맵]]**
- **[[📂 01_Genesis_NMSJ/초기_플롯_조각_모음_NMSJ.md|초기 플롯 조각 모음]]**
- **[[주인공_기록자_내러티브_강화안_NMSJ]]** (옵시디언 내 별도 노트로 저장 후 링크 권장 - 예: `/01_Genesis_NMSJ/`)
- **[["내가 먹물로 새기는 전설" - 최종 보스 서사 강화안]]** (옵시디언 내 별도 노트로 저장 후 링크 권장 - 예: `/01_Genesis_NMSJ/`)
- **[["내가 먹물로 새기는 전설" - 역사 배합 및 세계관 심화 전략]]** (옵시디언 내 별도 노트로 저장 후 링크 권장 - 예: `/01_Genesis_NMSJ/`)

---

## 🌍 로어 위버 (Lore Weaver) - 세계관 및 등장인물

- **[[📂 02_Lore_NMSJ/|➡️ 세계관 설정 폴더 바로가기]]**
    - **주요 아티팩트**:
        - `[[진묵_삼한비록지묵_설정_NMSJ]]`
        - `[[흑요_아사달의망령_설정_NMSJ]]`
    - **주요 세력**:
        - `[[화백회_설정_NMSJ]]`
        - `[[흑월단_설정_NMSJ]]`
        - (용비대, 국혼사 등 추가 예정)
    - **역사적 배경**: `[[고조선_삼한시대_역사_배경_설정_NMSJ]]`
- **[[📂 02_Lore_NMSJ/Characters_NMSJ/|➡️ 등장인물 폴더 바로가기]]**
    - **주인공**: `[[이도윤_주인공_NMSJ]]`
    - **핵심 조력자/대립자**: `[[골동품상_묵선생_NMSJ]]`, `[[진묵_목소리_캐릭터_NMSJ]]`
    - (Dataview 쿼리 예시: 최근 수정된 캐릭터 노트 3개)
      ```dataview
      LIST FROM "Author_Projects/Project_내가_먹물로_새기는_전설/02_Lore_NMSJ/Characters_NMSJ"
      SORT file.mtime DESC
      LIMIT 3
      ```

---

## 📜 내러티브 아키텍트 (Narrative Architect) - 플롯 및 아크

- **[[📂 03_Narrative_NMSJ/|➡️ 플롯 설계 폴더 바로가기]]**
- **[[📂 03_Narrative_NMSJ/전체_플롯_아크_개요_NMSJ.md|전체 플롯 아크 개요 (200화+)]]**
- **현재 아크**: `[[📂 03_Narrative_NMSJ/Arc_01_검은먹물의_각성_NMSJ/Arc01_Synopsis_NMSJ.md|1부: 검은 먹물의 각성 - 시놉시스]]`
    - `[[📂 03_Narrative_NMSJ/Arc_01_검은먹물의_각성_NMSJ/Arc01_Event_List_NMSJ.md|1부 상세 이벤트 리스트 (1~5화 빌드업 강화 버전)]]`
- **[[📂 03_Narrative_NMSJ/떡밥_리스트_및_회수_계획_NMSJ.md|떡밥 리스트 및 회수 계획]]**

---

## ✍️ 코라이팅 스튜디오 (Co-Writing Studio) - 원고 집필 현황

- **[[📂 04_Manuscript_NMSJ/|➡️ 원고 폴더 바로가기]]**
- **최근 원고**:
    - `[[📂 04_Manuscript_NMSJ/EP01_NMSJ/1화_검은재앙_피로쓰다_NMSJ.md|1화: 검은 재앙, 피로 쓰다 (작가님 작성본)]]`
    - `[[📂 04_Manuscript_NMSJ/EP02_NMSJ/2화_기록자의혈손_첫번째시험_NMSJ.md|2화: 기록자의 혈손, 그리고 첫 번째 시험 (작가님 작성본)]]`
- **다음 집필 대상**: 제3화
- (Dataview 쿼리 예시: '집필 중' 상태인 원고 목록)
  ```dataview
  TABLE episode_number AS "회차", title AS "제목", current_word_count AS "현재분량", pov_character AS "시점인물"
  FROM "Author_Projects/Project_내가_먹물로_새기는_전설/04_Manuscript_NMSJ"
  WHERE contains(type, "manuscript") AND contains(status, "writing")
  SORT episode_number ASC
```

## 📊 프로젝트 현황

### 현재 단계
- **Phase**: 2 - 초기 데이터 입력 단계
- **현재 아크**: 1부 검은 먹물의 각성
- **다음 마일스톤**: 프로젝트 초기 데이터 입력 완료 및 3화 집필 착수

### 핵심 문서 연결
- **프로젝트 개요**: [[00_프로젝트_개요_NMSJ/프로젝트_개요_NMSJ]]
- **세계관 설정**: [[02_Lore_NMSJ/세계관_설정_NMSJ]]
- **플롯 구조**: [[03_Narrative_NMSJ/전체_플롯_아크_개요_NMSJ]]
- **원고 관리**: [[04_Manuscript_NMSJ/원고_관리_NMSJ]]

### CMDS 연결
- **엔진 핵심**: [[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Storyweaver_Engine_HQ]]
- **범용 원칙**: [[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/CMDS_Universal_Principles]]
- **스타일 가이드**: [[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Author_Style_Guide_Main]]