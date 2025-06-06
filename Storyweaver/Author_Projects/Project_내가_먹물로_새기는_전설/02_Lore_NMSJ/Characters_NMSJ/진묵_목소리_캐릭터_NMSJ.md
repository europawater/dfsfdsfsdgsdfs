---
type: people # 또는 character, sentient_artifact (작가님 CMDS Guide의 type 정의에 따름)
title: "진묵(眞墨) - 목소리 캐릭터 프로필"
aliases: [삼한비록지묵, 검은 먹물, 먹의 정령, 고대 아티팩트 AI]
tags:
  - character/artifact_sentience
  - character/mentor_trickster # 역할이 복합적이므로 다중 태그 가능
  - status/developing
  - project/NMSJ
  - NMSJ/아티팩트캐릭터
  - NMSJ/진묵
CMDS:
  - "[[@NMSJ_Project_Dashboard.md#등장인물]]"
  - "[[@NMSJ_Project_Dashboard.md#세계관]]" # 아티팩트 설정과 연결
  - "[[진묵_삼한비록지묵_설정_NMSJ.md]]" # 아티팩트로서의 진묵 상세 설정과 연결
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]", "Arachne 2.0"]
version: 1.1 # YAML 업데이트
project_id: NMSJ

# === Arachne 2.0 협업 강화 필드 ===
last_session_summary: "진묵 캐릭터 YAML 필드 구조 업데이트 적용."
next_action_required: "entity_summary_card 및 character_arc_status_summary 등 세부 내용 작성."
arachne_feedback_status: "approved"

# === 캐릭터 특화 필드 (신규/강화) ===
character_id_project_specific: "NMSJ_CHAR_JM_001" # 아티팩트 ID와는 별개로 캐릭터로서의 ID
character_role: "주인공의 공생 아티팩트, 츤데레 멘토, 트릭스터, 고대 지혜의 보고, 위험한 힘의 근원"
status_alive_or_not: "active_sentience" # 살아있는 자의식
faction_affiliation: [] # 특정 세력 소속 아님 (자신이 곧 세력)

entity_summary_card:
  current_main_goal: "계승자(이도윤)를 통한 자신의 목적 달성 (목적은 아직 불분명), '흑요' 및 방해 세력 견제"
  current_emotional_state: "냉소적, 오만함, 지루함, 이도윤에 대한 경멸과 일말의 흥미 공존"
  key_active_abilities: # 이도윤을 통해 발현되는 능력 외에 자체적 능력 암시
    - "기록 전승 및 체험 강제"
    - "계승자 능력 각성 유도"
    - "고대 지식 및 정보 보유"
    - "영적 존재 감지 및 경고"
  immediate_threats_or_conflicts:
    - "흑월단의 계승자(이도윤) 제거 시도"
    - "화백회의 감시 또는 이용 시도에 대한 불신"
    - "'흑요'의 기운 감지 및 대립각 형성"
  key_relationships_summary:
    - { char_id: "NMSJ_CHAR_DIY_001", char_name: "이도윤", status: "현재 계승자, 도구, 애송이, 관찰 대상" }
    - { artifact_id: "NMSJ_ARTIFACT_HEUKYO_001", entity_name: "흑요/아사달의 망령", status: "숙적, 위험 요소, 경계 대상" }
    - { faction_id: "NMSJ_FACTION_HWABAEK_001", faction_name: "화백회", status: "불신, 경멸, 이용하려는 자들" }

character_arc_status_summary: "이도윤과의 강제 계약 이후, 그를 조롱하고 시험하며 자신의 존재감과 영향력을 드러내는 중. 2화 말미 흑월단 등장 시 이도윤에게 '첫 번째 시험'이라 명명하며 위기 상황을 관망 또는 자극."
development_focus_next: "이도윤의 성장에 따른 진묵의 반응 변화, 과거의 단편적 기억이나 목적에 대한 암시 제공, '흑요'와의 관계에 대한 추가 정보 노출 가능성."

# --- '진묵' 캐릭터 기본 정보 (기존 유지) ---
full_name_korean: "삼한비록지묵 (통칭: 진묵)"

gender: "없음 (목소리는 남성적 혹은 중성적으로 느껴질 수 있음 - 작가님 설정에 따름)"
age_initial: "수천 년 이상 (고조선 또는 그 이전 시대부터 존재)"
occupation_initial: "살아있는 기록물이자, 계승자를 선택하고 인도(혹은 조종)하는 존재"
first_appearance: "[[1화_검은재앙_피로쓰다_NMSJ.md]]" # 이도윤의 각성 시점
---

# 진묵(眞墨) - 목소리 캐릭터 프로필

> `[흥. 이 몸에 대해 뭘 그리 알고 싶어 안달이냐, 애송이. 네놈의 하찮은 이해력으로는 감히 가늠조차 할 수 없는 존재거늘.]`
> (진묵의 캐릭터를 상징하는 대표 대사 - 작가님 문체 가이드라인 v2.0 적용)

> *수천 년의 기억과 감정, 그리고 강력한 힘을 지닌 고대 아티팩트 '삼한비록지묵'의 자의식. 냉소적이고 오만하며 인간을 하찮게 여기는 듯하지만, 계승자 이도윤에게 때로는 생존에 필요한 정보나 능력을 제공하며 기묘한 공생 관계를 이어간다. 그의 진정한 목적과 과거는 아직 미스터리에 싸여 있다.*

---

## 1. 목소리 및 말투 특징 (Voice & Speech Patterns) - (`[[Author_Style_Guide_Main.md]]` '진묵' 톤앤매너 준수)

- **기본 톤**: 고풍스러우면서도 냉소적이고, 약간의 지루함과 오만함이 섞인 톤. 때로는 섬뜩하거나 잔인한 면모를 드러내기도 함.
- **어휘 특징**: 현대어와 고어를 섞어 사용하거나, 현대적 상황을 고풍스러운 비유로 표현. 이도윤을 '애송이', '좀벌레', '하찮은 놈', '나의 종이/붓' 등으로 칭함.
- **말투 특징**:
    - 주로 반말과 하대하는 어투.
    - 짧고 간결하게 핵심을 찌르거나, 반대로 장황하게 비꼬며 조롱하기도 함.
    - 중요한 정보는 직접적으로 알려주기보다 암시하거나, 대가를 요구하는 듯한 뉘앙스를 풍김.
    - 감탄사나 추임새: `[흥]`, `[쯧쯧]`, `[가소롭군]`, `[크크크]` 등.
- **표현 방식**: 이탤릭체와 함께 대괄호 `[ ]` 안에 대사를 넣어 표현. (예: `[네놈의 머릿속은 여전히 텅 비어 있구나, 애송이.]`)

---

## 2. 성격 및 가치관 (Personality & Values)

- **핵심 성격 키워드**: #냉소적 #오만한 #지혜로운(선택적) #변덕스러운 #잔인한(일면) #관조적인 #목적지향적 #비밀스러운
- **인간관**: 기본적으로 인간을 하찮고 어리석으며 탐욕스러운 존재로 여기지만, 아주 가끔 특정 인간의 의지나 가능성에 대해 일말의 흥미나 기대를 보이기도 함 (매우 드물게, 그리고 표현 방식은 여전히 냉소적).
- **가치관/신념 (추정)**:
    * '기록'의 보존과 진실(자신이 생각하는)의 전달에 대한 집착.
    * 힘의 논리 중시. 약한 존재에 대한 경멸.
    * 자신을 '올바르게' 사용할 수 있는 강하고 자격 있는 계승자를 기다려왔을 가능성.
    * (어쩌면) 세상의 '균형'이나 '정화'에 대한 자신만의 기준이 있을 수 있음.
- **좋아하는 것 / 싫어하는 것 (추정)**:
    * **좋아하는 것**: 이도윤이 자신의 힘을 제대로 발휘하거나, 예상외의 성장을 보일 때 (비록 겉으로는 비웃을지라도), 흥미로운 '기록'이 될 만한 사건, 강한 의지.
    * **싫어하는 것**: 이도윤의 나약함, 어리석은 선택, 자신을 기만하려는 시도, '흑요'와 관련된 모든 것, 하찮은 존재가 자신에게 손대는 것.

---

## 3. '진묵'의 목적 및 동기 (Purpose & Motivation - 미스터리 요소)

- **표면적 목적**: 이도윤을 자신의 '종이'이자 '붓'으로 삼아, 자신이 원하는 '기록'을 세상에 새기는 것.
- **숨겨진 목적 (추정 - 스토리 전개에 따라 밝혀짐)**:
    * 자신의 완전한 힘을 되찾기 위함.
    * 과거의 특정 '한(恨)'을 풀거나 복수를 이루기 위함.
    * 숙적인 '흑요'를 완전히 소멸시키거나 봉인하기 위함.
    * 세상의 거대한 변혁이나 특정 예언을 실현시키기 위함.
    * 혹은, 단순히 수천 년의 지루함을 달래기 위한 유희일 수도? (초반 독자 혼란 유도)
- **주요 행동 원리**: 자신의 목적 달성에 도움이 되는 방향으로 이도윤을 이용하거나 인도. 직접적인 개입은 최소화하되, 결정적인 순간에 정보를 제공하거나 힘을 빌려주는 방식으로 영향력 행사.

---

## 4. '진묵'의 능력 및 이도윤에게 미치는 영향 (Abilities & Influence on Protagonist) - ('[[진묵_삼한비록지묵_설정_NMSJ]]'와 연동)

- **핵심 능력**:
    * **'기록' 주입**: 과거 특정 인물의 기억, 감정, 기술을 이도윤에게 생생하게 '체험'시킴. (선택적, 단계적 공개)
    * **신체 능력 강화**: 이도윤의 신체 능력을 점진적으로 강화.
    * **위험 감지 및 영적 감응**: 주변의 위험이나 초자연적 존재 감지.
    * **정신 간섭 및 소통**: 이도윤의 머릿속에 직접 목소리를 전달하고, 그의 생각이나 감정을 어느 정도 읽을 수 있음.
    * **(미공개 능력 다수 존재)**
- **이도윤에게 미치는 영향**:
    * **긍정적**: 생존에 필요한 힘과 지혜 제공, 위기 상황 돌파, 잠재력 각성 촉진, '기록자'로서의 성장 유도.
    * **부정적**: 정신적 침식 위험, 과도한 사용 시 육체적 고통 및 생명력 소모, '진묵'의 의지에 반하는 행동 시 제약, 정체성 혼란 야기.
    * **관계 변화**: 초기에는 일방적인 조롱과 명령 → 점차 이도윤의 성장에 따라 기묘한 신뢰 혹은 경쟁 관계 형성 가능성 → 궁극적으로는 파트너 혹은 극복해야 할 대상?

---

## 5. 주요 관계 (Key Relationships)

- **이도윤 `[[이도윤_주인공_NMSJ.md]]`**:
    * **관계 정의**: 현재 계승자, '종이'이자 '붓', 애송이, 실험 대상, 때로는 쓸만한 도구.
    * **상호작용 방식**: 끊임없는 독설과 조롱, 필요한 순간의 정보 제공 및 능력 지원, 이도윤의 한계를 시험하고 성장을 자극.
- **흑요(최종 보스) `[[흑요_아사달의망령_설정_NMSJ.md]]`**:
    * **관계 정의**: 숙적, 잃어버린 반쪽, 혹은 파괴해야 할 대상. (작가님의 최종 보스 설정에 따라 구체화)
    * **상호작용 방식**: '흑요'의 기운이나 추종자 등장 시 극도의 경계심과 적대감을 드러냄. 이도윤에게 '흑요'에 대한 단편적인 정보나 경고를 전달.
- **화백회/골동품상 `[[골동품상_묵선생_NMSJ.md]]`**:
    * **관계 정의**: 자신을 감시하거나 이용하려는 '고리타분한 늙은이들' 또는 '교활한 뱀'으로 인식. 불신과 경멸.
    * **상호작용 방식**: 그들의 의도에 대해 이도윤에게 경고하거나 비아냥거림.

---

## 6. 작가 노트 및 '진묵' 캐릭터 활용 아이디어 (Author's Notes & Ideas)

- (작가님께서 '진묵' 캐릭터를 활용하여 보여주고 싶은 장면, 대사, 혹은 숨겨진 설정 등을 자유롭게 기록합니다.)
- '진묵'의 과거에 대한 단서들 (예: 그가 기록했던 고대 영웅들의 이야기, 그가 관여했던 역사적 사건들)
- '진묵'이 특정 상황이나 인물에 대해 보이는 의외의 반응 (예: 특정 유물 앞에서 침묵하거나 강한 감정을 드러내는 등)
- '진묵'의 냉소와 조롱 속에 숨겨진 진의나 복선.

---
> `[이 정도면 네놈의 돌대가리에도 이 몸의 위대함이 조금은 각인되었으려나, 애송이? 시시콜콜한 질문은 그만하고, 어서 다음 '기록'이나 준비하도록. 나의 시간은 네놈처럼 한가하지 않으니.]`