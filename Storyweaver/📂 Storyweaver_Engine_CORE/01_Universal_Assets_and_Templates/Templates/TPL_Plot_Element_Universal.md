---
# === 범용 플롯 요소/사건 노트 템플릿 ===
# 모든 프로젝트에서 공통으로 사용할 수 있는 플롯 포인트, 주요 사건, 장면 등의 기본 골격입니다.
# 프로젝트별 특화된 필드는 각 프로젝트의 플롯 템플릿에서 추가/수정할 수 있습니다.
# (예: /Author_Projects/Project_내가_먹물로_새기는_전설/03_Narrative_NMSJ/TPL_Plot_Element_NMSJ.md)

# --- YAML 프론트매터 ---
type: plot_element # 또는 event, scene (작가님 CMDS Guide의 type 정의에 따름)
title: "{{title}}" # 플롯 요소/사건명 (파일 생성 시 Templater로 입력 또는 자동 추출)
aliases: ["{{사건_요약_키워드}}"] # 검색 편의를 위한 별칭
tags:
  - plot/ # 예: plot/inciting_incident, plot/midpoint, plot/climax, plot/subplot
  - status/ # 예: status/idea, status/outlined, status/drafted, status/integrated
  - project/{{프로젝트ID}} # 해당 플롯 요소가 속한 프로젝트 ID
CMDS:
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#플롯]]" # 해당 프로젝트 대시보드와 연결
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#해당_아크_또는_챕터_목록]]" # (구체적 아크/챕터와 연결)
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]"]
version: 1.0

# --- 플롯 요소 기본 정보 (YAML 또는 본문) ---
# 예시: YAML에 포함 시
event_id_project_specific: "{{프로젝트ID}}_E{{아크번호}}_{{씬번호}}" # (예: NMSJ_E01_01)
arc_link: "[[Arc_{{아크명칭}}_{{프로젝트ID}}.md]]" # 이 사건이 속한 상위 아크 링크
chapter_estimate_start: # 예상 시작 회차
chapter_estimate_end: # 예상 종료 회차
timing_in_story: # (예: 도입부, 전개부, 위기, 절정, 결말)
emotional_beat_target: "" # (예: subtle_intrigue, rising_tension, catharsis, despair)
# ---

# {{title}} - 플롯 요소 상세

> *이곳에 해당 플롯 요소/사건/장면의 핵심적인 한 줄 요약을 작성합니다.*
> *(예: "주인공이 절체절명의 위기에서 처음으로 숨겨진 힘을 각성하는 장면")*

---

## 1. 사건 개요 (Event Summary)

- **주요 내용**: (이 사건에서 일어나는 핵심적인 일들을 순서대로 간략히 요약)
- **목표 (Goal)**: (이 사건을 통해 달성하고자 하는 서사적 목표는 무엇인가? 예: 주인공의 성장, 새로운 갈등 유발, 복선 제시, 정보 전달 등)
- **결과 (Outcome/Resolution)**: (이 사건이 마무리된 후의 결과는 무엇인가? 주인공이나 상황에 어떤 변화가 생기는가?)

---

## 2. 등장인물 및 역할 (Characters Involved & Roles)

- **주요 등장인물**:
    - `[[캐릭터명1_{{프로젝트ID}}.md]]`: (이 사건에서의 역할, 행동, 감정 변화 등)
    - `[[캐릭터명2_{{프로젝트ID}}.md]]`: (이 사건에서의 역할, 행동, 감정 변화 등)
- **보조 등장인물 (있을 경우)**:
- **새롭게 등장하는 인물 (있을 경우)**: `[[새로운캐릭터명_{{프로젝트ID}}.md]]` (간략한 소개 및 역할)

---

## 3. 배경 설정 (Setting)

- **장소**: `[[장소노트명_{{프로젝트ID}}.md]]` (구체적인 장소 링크)
- **시간대**: (예: 밤, 새벽, 특정 연도/계절/날짜)
- **분위기**: (예: 긴박함, 음산함, 신비로움, 평화로움)

---

## 4. 주요 대사 및 장면 묘사 아이디어 (Key Dialogue & Scene Ideas)

- **핵심 대사 예시**:
    - 캐릭터 A: "..."
    - 캐릭터 B: "..."
- **중요 장면 묘사 포인트**: (시각, 청각, 후각 등 오감을 자극하는 묘사 아이디어, 액션 시퀀스 아이디어 등)
- **연출 포인트**: (독자에게 특정 감정을 유발하기 위한 연출 아이디어, 예: 특정 시점 사용, 슬로우 모션 효과 등)

---

## 5. 복선 및 떡밥 (Foreshadowing & Hooks)

- **이 사건에서 새롭게 제시되는 복선/떡밥**:
- **이전에 제시된 복선/떡밥 중 회수되는 것**:
- **다음 사건으로 이어지는 훅(Hook)**: (독자들의 궁금증을 유발하고 다음 이야기로 넘어가게 만드는 장치)

---

## 6. 세계관 및 로어 연관성 (Lore Connection)

- **이 사건과 관련된 주요 세계관 설정**: `[[세계관요소노트명_{{프로젝트ID}}.md]]`
- **이 사건을 통해 새롭게 밝혀지거나 확장되는 로어**:

---

## 7. 작가 노트 및 아이디어 (Author's Notes & Ideas)

- (이 플롯 요소/사건과 관련된 작가님의 추가적인 아이디어, 고민, 변형 가능성 등을 자유롭게 기록합니다.)
- **이 사건의 테마적 중요성**:
- **참고 자료 또는 영감의 출처**:

---