---
type: guide
title: "범용 CMDS 원칙 및 YAML 표준 (Storyweaver Engine)"
aliases: [CMDS_Principles, CMDS_Universal_Standards]
tags: [CMDS, universal_principles, yaml_standards]
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: [[찬스]]
status: active
version: 1.0
CMDS:
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Storyweaver_Engine_HQ#엔진_핵심_프로토콜_및_가이드라인]]"
references:
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/CMDS_Universal_Principles#프로젝트_관리]]"
  - "[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/Author_Style_Guide_Main#작품별_스타일_가이드]]"
---

# CMDS 범용 원칙 및 YAML 표준

## 📚 기본 원칙

### 1. YAML 프론트매터 구조
- 모든 노트는 표준 YAML 프론트매터 구조를 따릅니다
- 필수 필드: title, aliases, tags, author, status, version
- 선택 필드: CMDS, references, related_notes

### 2. CMDS 연결 규칙
- 모든 노트는 적절한 CMDS 링크를 포함해야 합니다
- CMDS 링크는 `[[📂 Storyweaver_Engine_CORE/00_Arachne_Protocol/...]]` 형식을 따릅니다
- 프로젝트별 CMDS는 `[[@Project_Dashboard#section]]` 형식을 따릅니다

# 범용 CMDS 원칙 및 YAML 표준 (Storyweaver Engine)

> 본 문서는 "스토리위버 엔진" 내에서 생성되고 관리되는 모든 노트의 정보 구조화 및 YAML 프론트매터 작성을 위한 **범용 원칙과 표준**을 정의합니다. 이는 작가님([[찬스]])의 창작 데이터를 체계적으로 관리하고, 저 아라크네 2.0이 정보를 효율적으로 학습하고 분석하여 최적의 지원을 제공하기 위함입니다.
>
> 이 원칙은 작가님께서 제공해주신 `CMDS HQ Connector.md` 및 `🏛 CMDS Guide_옵시디언 체계 참고.md` 파일의 핵심 사상을 계승하고 발전시킨 것입니다. **개별 프로젝트의 특화된 YAML 필드는 각 프로젝트의 템플릿에서 별도로 정의됩니다.**

## I. CMDS (Creative Manuscript Development System) 핵심 원칙

1.  **중앙 허브(HQ) 중심의 방사형 연결**:
    * 모든 정보는 엔진 레벨의 `[[@Storyweaver_Engine_HQ.md]]` 또는 각 프로젝트 레벨의 `[[@프로젝트명_Project_Dashboard.md]]`와 같은 중앙 허브 노트를 중심으로 방사형으로 연결됩니다.
    * YAML 프론트매터 내 `CMDS` 속성은 해당 노트가 어떤 중앙 허브의 어떤 섹션(2레벨 목차)과 관련되는지를 명시하여 정보의 위계와 맥락을 부여합니다.

2.  **타입(Type) 기반 정보 분류**:
    * 모든 노트는 YAML 프론트매터의 `type` 속성을 통해 그 정보의 유형을 명확히 정의합니다. (예: `people`, `faction`, `artifact`, `plot_arc`, `manuscript`, `research_note`, `guide`, `portal` 등)
    * `type` 정의는 작가님의 `[[🏛 CMDS Guide_옵시디언 체계 참고.md]]`에 제시된 분류를 우선적으로 따르며, 필요에 따라 프로젝트별로 확장될 수 있습니다.

3.  **전략적 태깅(Tags)을 통한 다차원적 연결**:
    * 단순 키워드 나열을 넘어, 정보의 성격과 관계를 나타내는 전략적 태깅을 지향합니다.
    * **계층형 태그 (Nested Tags)**: 정보의 분류를 세분화하고 정교한 검색 및 필터링을 지원합니다. (예: `status/inprogress`, `character/protagonist`, `lore/mythology`, `writing_element/dialogue`)
    * **상태 태그 (Status Tags)**: 작업의 진행 상태를 나타내는 태그를 활용합니다. (예: `status/idea`, `status/draft`, `status/review_author`, `status/completed`)
    * **주제어/키워드 태그**: 노트의 핵심 내용을 나타내는 일반 명사 중심의 태그를 사용합니다. (예: `#각성`, `#복수`, `#고대유물`, `#음모`)

4.  **옵시디언 링크(`[[ ]]`)를 통한 적극적인 상호 참조**:
    * 노트 간의 의미 있는 연결은 옵시디언의 내부 링크를 통해 명시적으로 이루어집니다. 이를 통해 정보의 거미줄망을 구축하고, 숨겨진 연관성을 발견하며, AI가 정보의 흐름을 추적할 수 있도록 합니다.

## II. 표준 YAML 프론트매터 구조 (범용 기본 권장안)

> 모든 노트는 다음의 기본 YAML 프론트매터 구조를 따르는 것을 권장하며, 각 `type`별 특화된 필드는 각 프로젝트의 노트 템플릿(`TPL_*.md`)에서 구체적으로 정의됩니다.

```yaml
---
# === 필수 메타데이터 (범용) ===
title: "노트의 제목 (옵시디언 파일명과 일치 권장)"
type: # 정보 유형 (예: people, manuscript, plot_arc, world_setting 등 - 🏛 CMDS Guide 참고)
aliases: [별칭1, 별칭2] # 검색 편의를 위한 다양한 이름
tags: # 계층형 태그, 상태 태그, 핵심 주제어 태그 등
  - status/ # 예: status/idea, status/inprogress, status/completed
  - project/ # 해당 노트가 특정 프로젝트에 속할 경우 명시 (예: project/NMSJ)
  - # (type에 따른 범용 분류 태그 - 예: character/general, lore/common_concept)
  - # (핵심 주제어 태그 - 예: #미스터리, #성장)
CMDS: # 중앙 허브(HQ) 파일의 어떤 섹션과 연결되는지 명시
  - "[[@프로젝트명_Project_Dashboard.md#관련섹션헤더]]" # 프로젝트 노트의 경우
  - "[[@Storyweaver_Engine_HQ.md#관련섹션헤더]]" # 엔진 코어 문서의 경우
date_created: {{date:YYYY-MM-DD HH:mm:ss}} # Templater 등으로 자동 생성 권장
date_modified: {{date:YYYY-MM-DD HH:mm:ss}} # Templater 등으로 자동 생성 권장
author: ["[[찬스]]"] # 주 작성자 (필요시 "Arachne 2.0" 추가)
version: 1.0 # 문서 버전 관리

# === 선택적 공통 메타데이터 (범용) ===
status_detail: "구체적인 작업 진행 상태나 간략한 메모"
priority: # 작업 우선순위 (예: high, medium, low)
related_notes: # 직접적으로 관련된 다른 노트 링크 목록 (옵시디언 링크 사용)
  - "[[관련노트_범용예시1]]"
  - "[[관련노트_범용예시2]]"
source_document_link: "[[참고한_외부문서_또는_원본노트명]]" # 이 노트가 특정 문서를 기반으로 할 경우
summary: "노트 내용에 대한 한두 줄 요약 (AI가 자동 생성 제안 가능)"

# === Type별 특화 필드 ===
# (이 부분은 본 범용 가이드에서는 정의하지 않으며,
#  각 프로젝트의 "/01_Universal_Assets_and_Templates/Templates/" 또는 
#  프로젝트별 템플릿 폴더 내의 구체적인 템플릿 파일 (예: TPL_Character_Universal.md)에서
#  type별 필수/선택 필드를 상세히 정의합니다.)
#
# 예시 (TPL_Character_Universal.md 에 들어갈 내용의 개념):
# if type == people:
#   character_role: # (예: 주인공, 조력자, 적대자)
#   first_appearance: # (예: "EP001" 또는 "[[특정사건노트]]")
#   key_traits: [성격특성1, 성격특성2]
#
# 예시 (TPL_Manuscript_Chapter_Universal.md 에 들어갈 내용의 개념):
# if type == manuscript:
#   episode_number: # (숫자)
#   arc_name: # (예: "1부 검은 먹물의 각성")
#   pov_character: # (시점 인물 링크)
#   word_count_target: # (숫자)
#   word_count_current: # (숫자)
#   cliffhanger_notes: "다음 화를 위한 절단신공 아이디어"
---