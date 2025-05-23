---
# === 범용 세계관 설정 요소 템플릿 ===
# 모든 프로젝트에서 공통으로 사용할 수 있는 세계관의 특정 요소(지역, 조직, 아이템, 개념 등)를 정의하는 기본 골격입니다.
# 프로젝트별 특화된 필드는 각 프로젝트의 세계관 템플릿에서 추가/수정할 수 있습니다.
# (예: /Author_Projects/Project_내가_먹물로_새기는_전설/02_Lore_NMSJ/TPL_World_Setting_NMSJ.md)

# --- YAML 프론트매터 ---
type: world_setting # 또는 lore_element, faction, location, item, concept (작가님 CMDS Guide의 type 정의에 따름)
title: "{{title}}" # 세계관 요소명 (파일 생성 시 Templater로 입력 또는 자동 추출)
aliases: ["{{설정_다른이름_또는_약칭}}"] # 검색 편의를 위한 별칭
tags:
  - lore/ # 예: lore/location, lore/faction, lore/artifact, lore/magic_system, lore/historical_event
  - status/ # 예: status/idea, status/developing, status/finalized
  - project/{{프로젝트ID}} # 해당 설정 요소가 속한 프로젝트 ID
CMDS:
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#세계관]]" # 해당 프로젝트 대시보드와 연결
  - "[[@{{프로젝트ID}}_Project_Dashboard.md#관련_상위_세계관_분류_링크]]" # (예: #주요_세력_및_조직)
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]"]
version: 1.0

# --- 세계관 요소 기본 정보 (YAML 또는 본문) ---
# 예시: YAML에 포함 시
setting_id_project_specific: "{{프로젝트ID}}_LORE_{{요소_ID}}" # (예: NMSJ_LORE_JINMUK)
category: "" # (예: 아티팩트, 조직, 지역, 역사적 사건, 마법체계, 문화, 종족 등)
significance_level: # (예: major, minor, background)
first_mentioned_in: "EP000" # (처음 언급/등장하는 에피소드 번호 또는 링크)
# ---

# {{title}} - 세계관 설정 상세

> *이곳에 해당 세계관 요소의 핵심적인 한 줄 요약이나 중요도를 간략히 기술합니다.*
> *(예: "고대 삼한시대에 피와 한으로 빚어진, 살아있는 저주받은 먹 '삼한비록지묵'")*

---

## 1. 기본 개요 (Overview)

- **정의 및 설명**: (이 세계관 요소는 무엇인가? 핵심적인 특징은?)
- **기원 및 역사**: (언제, 어떻게 생겨났거나 만들어졌는가? 주요 역사적 배경은?)
- **외형 또는 주요 특징**: (물리적 형태, 상징, 주요 능력, 작동 방식 등 구체적인 묘사)

---

## 2. 작품 내 역할 및 기능 (Role and Function in Story)

- **주요 역할**: (이 설정 요소가 이야기 전체 또는 특정 아크/에피소드에서 수행하는 핵심적인 역할은 무엇인가?)
- **주인공 및 다른 캐릭터와의 관계**: (주인공이나 다른 주요 인물들과 어떤 관계를 맺고 있는가? 어떤 영향을 주고받는가?)
- **플롯 전개에 미치는 영향**: (이 설정 요소가 주요 사건이나 플롯의 흐름에 어떤 식으로 기여하거나 영향을 미치는가?)

---

## 3. 세부 설정 및 규칙 (Detailed Settings & Rules)

- (이 항목은 설정 요소의 `category`에 따라 내용이 크게 달라질 수 있습니다. 아래는 예시입니다.)
- **만약 `category: 아티팩트` 라면**:
    - `능력 상세`:
    - `사용 조건 및 대가/제약`:
    - `제작 과정 또는 재료 (알려진 경우)`:
    - `현재 소유자 또는 위치`:
- **만약 `category: 조직/세력` 이라면**:
    - `목표 및 이념`:
    - `주요 구성원 및 리더`: `[[캐릭터명1_{{프로젝트ID}}.md]]`, `[[캐릭터명2_{{프로젝트ID}}.md]]`
    - `세력 규모 및 영향력`:
    - `다른 조직과의 관계`: (우호, 적대, 중립 등)
    - `주요 활동 영역 및 방식`:
- **만약 `category: 지역/장소` 라면**:
    - `지리적 위치 및 환경`:
    - `주요 특징 및 랜드마크`:
    - `역사적 중요성 또는 관련 사건`:
    - `거주민 또는 관련 인물`:
- **만약 `category: 마법체계/능력시스템` 이라면**:
    - `기본 원리 및 법칙`:
    - `능력의 종류 및 등급`:
    - `습득 조건 및 수련 방법`:
    - `한계 및 부작용`:

---

## 4. 관련된 다른 세계관 요소 (Related Lore Elements)

- `[[다른_세계관_요소_노트명1_{{프로젝트ID}}.md]]`: (연관성 설명)
- `[[다른_세계관_요소_노트명2_{{프로젝트ID}}.md]]`: (연관성 설명)
- (필요에 따라 연관 요소 항목 추가)

---

## 5. 미스터리 및 떡밥 (Mysteries & Foreshadowing)

- **이 설정 요소와 관련된 풀리지 않은 의문점이나 비밀**:
- **향후 스토리에 영향을 미칠 수 있는 잠재적인 떡밥**:

---

## 6. 작가 노트 및 아이디어 (Author's Notes & Ideas)

- (이 세계관 요소와 관련된 작가님의 추가적인 아이디어, 영감의 출처, 변형 가능성 등을 자유롭게 기록합니다.)
- **이 설정을 통해 전달하고 싶은 테마적 요소**:
- **참고 자료 (역사, 신화, 과학 등)**:

---