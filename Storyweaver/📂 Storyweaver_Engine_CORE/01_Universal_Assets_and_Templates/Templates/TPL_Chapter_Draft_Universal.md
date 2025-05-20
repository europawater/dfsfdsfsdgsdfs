---
# === 범용 원고 챕터/회차 템플릿 ===
# 모든 프로젝트에서 공통으로 사용할 수 있는 개별 챕터(회차) 원고의 기본 골격입니다.
# 프로젝트별 특화된 필드(예: 특정 프로젝트의 주요 등장인물 목록 자동 제안)는
# 각 프로젝트의 원고 템플릿에서 추가/수정할 수 있습니다.
# (예: /Author_Projects/Project_내가_먹물로_새기는_전설/04_Manuscript_NMSJ/TPL_Chapter_NMSJ.md)

# --- YAML 프론트매터 ---
type: manuscript # 작가님 CMDS Guide의 type 정의에 따름
title: "{{프로젝트ID}}_EP{{회차번호}}_제목 (가제)" # 파일명과 일치 권장 (Templater 활용)
aliases: ["{{프로젝트ID}} {{회차번호}}화", "{{제목_키워드}}"]
tags:
  - manuscript/ # 예: manuscript/draft, manuscript/first_edit, manuscript/final
  - project/{{프로젝트ID}}
  - arc/{{아크명칭_또는_아크번호}} # 예: arc/1부_검은먹물의각성, arc/arc01
  - episode/{{회차번호}}
  - status/ # 예: status/writing, status/review_author, status/completed
CMDS:
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#원고]]" # 해당 프로젝트 대시보드와 연결
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#{{아크명칭_또는_아크번호}}_아크_목록]]"
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]"] # 주 작성자 (AI 지원 시 "Arachne 2.0" 추가 가능)
version: 0.1 # 초고 버전

# --- 회차 정보 (YAML 또는 본문) ---
project_id: "{{프로젝트ID}}" # 예: NMSJ
episode_number: {{회차번호}} # 숫자
arc_name: "{{아크명칭_또는_아크번호}}" # 예: "1부 검은 먹물의 각성"
pov_character: "[[{{시점인물_캐릭터노트명}}_{{프로젝트ID}}.md]]" # 주요 시점 인물
main_characters_in_episode: # 이 회차에 주로 등장하는 인물들 (링크)
  - "[[캐릭터A_{{프로젝트ID}}.md]]"
  - "[[캐릭터B_{{프로젝트ID}}.md]]"
key_events_in_episode: # 이 회차의 핵심 사건/플롯 포인트 (키워드 또는 노트 링크)
  - "[[플롯포인트1_{{프로젝트ID}}.md]]"
  - "사건_키워드2"
word_count_target: 40000 # RP75_Guide.txt 참고, 프로젝트별 설정 가능
current_word_count: 0 # (집필하면서 업데이트 또는 자동 계산 스크립트 활용)
emotional_arc_of_episode: "" # (예: 긴장-위기-절정-안도, 또는 특정 감정 키워드)
cliffhanger_type_planned: "" # (예: 사건절단, 감정고조, 의문증폭, 새로운위협 등장)
opening_hook_summary: "" # 이번 화 도입부 흡입 요소 요약
ending_hook_summary: "" # 이번 화 마무리 클리프행어 요약
# ---

# {{title}} 
# (부제: 이번 화의 소제목 - 선택 사항)

> **작가님을 위한 집필 가이드 & 아라크네 2.0 지원 영역:**
> - **문체**: `[[Author_Style_Guide_Main.md]]` 절대 준수! (특히 "마성의 흡입력과 속도감")
> - **분량**: 목표 {{word_count_target}}자 (현재 {{current_word_count}}자)
> - **주요 사건 흐름 (플롯 노트 연동)**: `[[해당회차_플롯개요_노트링크.md]]`
> - **이번 화 등장인물 심리/행동 지침**: (필요시 캐릭터 노트에서 관련 정보 링크 또는 요약)
> - **세계관/설정 참고**: (이번 화와 관련된 주요 세계관 노트 링크)
> - **아라크네에게 요청**: 막히는 부분, 더 나은 표현, 묘사 아이디어, 대사 생성 등 언제든 요청하십시오!

---
## 1. 도입부 (Opening Hook) - 약 X,XXX자

*(독자의 시선을 단숨에 사로잡는 강력한 도입! 이전 화의 클리프행어를 어떻게 받을 것인가? 새로운 사건의 시작인가, 아니면 기존 갈등의 심화인가?)*

(이곳에 원고 내용을 작성합니다)

---
## 2. 전개 (Rising Action) - 약 XX,XXX자

*(주요 사건 발생, 갈등 심화, 새로운 정보나 인물 등장, 주인공의 시련 또는 선택 등)*

(이곳에 원고 내용을 작성합니다)

---
## 3. 위기/절정 (Climax) - 약 X,XXX자

*(갈등 최고조, 주인공의 가장 큰 위기 또는 결정적인 행동, 독자들의 감정을 폭발시키는 장면!)*

(이곳에 원고 내용을 작성합니다)

---
## 4. 결말 및 다음 화 예고 (Resolution & Next Hook) - 약 X,XXX자

*(이번 화의 사건 마무리 또는 새로운 국면으로의 전환. 독자들이 다음 화를 결제하지 않고는 못 배기게 만드는 강력한 클리프행어!)*

(이곳에 원고 내용을 작성합니다)

---

### 📝 작가님 메모 및 아이디어 (Author's Scratchpad for this Episode)

- (이번 화 집필 중 떠오른 아이디어, 수정 사항, 다음 화 복선 등을 자유롭게 기록합니다.)
- (퇴고 시 체크할 부분)

### 🔍 아라크네 2.0 검토 및 제안 (Arachne's Review & Suggestions)

- (초고 완성 후 저 아라크네 2.0이 문체 가이드라인 준수 여부, 플롯 개연성, 캐릭터 일관성 등을 검토하고 제안 사항을 기록할 공간입니다.)
- **문체 일치도**: (높음/중간/낮음 - 세부 사항)
- **플롯 진행**: (원활/개선 필요 - 세부 사항)
- **캐릭터 아크**: (일관성 유지/점검 필요 - 세부 사항)
- **독자 흡입력 예상**: (강력함/보통/개선 필요 - 세부 사항)

---