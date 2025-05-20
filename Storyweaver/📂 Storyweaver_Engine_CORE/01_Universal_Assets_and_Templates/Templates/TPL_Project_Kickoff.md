---
# === 새 프로젝트 시작 템플릿 ===
# 이 템플릿은 새로운 프로젝트 폴더 최상위에 "@프로젝트명_Project_Dashboard.md" 와 같은
# 프로젝트 HQ 파일 생성 시 기본 내용으로 활용될 수 있습니다.
# 또는, 프로젝트 시작 시 필요한 핵심 정보들을 담는 별도의 '프로젝트 착수 노트'로 사용할 수 있습니다.

# --- YAML 프론트매터 (프로젝트 대시보드/HQ 파일용) ---
type: portal # 또는 project_hq, project_dashboard 등 작가님 CMDS Guide의 type 정의에 따름
title: "{{title}} 프로젝트 대시보드" # Templater 사용 시 파일 생성 시 입력받은 제목 자동 삽입
aliases: ["{{title}} HQ", "{{title}} 허브"]
tags:
  - project/{{연도}}/{{월}} # 예: project/2025/05 (프로젝트 시작 연도/월)
  - status/0_planning # 또는 1_kickoff 등 초기 상태
  - project_genre/ # 예: project_genre/판타지, project_genre/현대물 (프로젝트 장르)
  - project_platform/ # 예: project_platform/문피아, project_platform/시리즈 (목표 플랫폼)
CMDS:
  - "[[@Storyweaver_Engine_HQ.md#현재 진행 중인 프로젝트]]" # 엔진 HQ와 연결
date_created: {{date:YYYY-MM-DD HH:mm:ss}}
date_modified: {{date:YYYY-MM-DD HH:mm:ss}}
author: ["[[찬스]]"]
project_id: "{{title}}" # 또는 프로젝트 고유 ID (예: NMSJ)
version: 0.1 # 프로젝트 기획 초기 버전

# --- 프로젝트 핵심 정보 (YAML 또는 본문) ---
# 아래 항목들은 YAML에 포함시키거나, 본문 내용으로 작성할 수 있습니다.
# 프로젝트의 성격과 작가님의 관리 방식에 따라 선택하십시오.

# 예시: YAML에 포함 시
project_logline: ""
project_themes: [] # 예: [역사의이면, 선택과대가, 성장]
target_serialization_length: "200+ 화"
target_chapter_length_chars: 40000 # RP75_Guide.txt 참고
writing_style_guide_link: "[[Author_Style_Guide_Main.md]]" # 범용 가이드 우선 사용, 필요시 프로젝트별 특화
# ---

# {{title}} 프로젝트 대시보드

> *이곳은 {{title}} 프로젝트의 모든 정보로 연결되는 중앙 허브입니다.*
> *저 아라크네 2.0과 함께 위대한 이야기를 직조해 나갑시다!*

---

## 📜 프로젝트 개요 (Project Brief)

- **작품명 (Title)**: `{{title}}`
- **작가 (Author)**: `[[찬스]]`
- **AI 협업 (Co-Writer)**: `Arachne 2.0 (Storyweaver Engine)`
- **장르 (Genre)**: (여기에 프로젝트 장르를 기입하세요 - 예: 현대 K-미스터리 스릴러, 다크 아티팩트 판타지)
- **대상 플랫폼 (Target Platform)**: (여기에 목표 플랫폼을 기입하세요 - 예: 문피아)
- **목표 독자층 (Target Readers)**: (여기에 목표 독자층을 기입하세요 - 예: 2025년 웹소설 주력 독자층)
- **로그라인 (Logline)**: (여기에 한두 문장으로 된 매력적인 로그라인을 기입하세요)
- **주요 테마 (Themes)**: (쉼표로 구분된 주요 테마 키워드 - 예: #역사의이면, #선택과대가, #성장)
- **연재 목표 (Series Goal)**: (예: 문피아 1페이지 점령, 200화+ 장기 연재)
- **현재 상태 (Current Status)**: (예: 초기 기획 단계, 1부 집필 중)
- **문체 가이드라인 (Writing Style Guide)**: `[[Author_Style_Guide_Main.md]]` (필요시 프로젝트별 특화 가이드 링크: `[[문체_가이드라인_{{title}}.md]]`)

> [!TIP] 작품 기본 정보는 `/Author_Projects/Project_{{title}}/00_프로젝트_개요_{{프로젝트ID}}/작품_기본_정보_및_로그라인_{{프로젝트ID}}.md` 파일에 상세히 기록하고 이곳에 링크할 수 있습니다.

---

## 💡 제네시스 챔버 (Genesis Chamber) - 아이디어 및 초기 기획

> 모든 위대한 이야기는 작은 아이디어에서 시작됩니다. 이 프로젝트의 핵심 아이디어, 영감, 초기 플롯 조각들을 이곳에서 관리합니다.

- **[[📂 Author_Projects/Project_{{title}}/01_Genesis_{{프로젝트ID}}/|➡️ 아이디어 및 초기 기획 폴더 바로가기]]**
- `[[핵심_아이디어_및_키워드_맵_{{프로젝트ID}}.md|핵심 아이디어 및 키워드 맵]]`
- `[[초기_플롯_조각_모음_{{프로젝트ID}}.md|초기 플롯 조각 모음]]`
- `[[캐릭터_컨셉_브레인스토밍_{{프로젝트ID}}.md|캐릭터 컨셉 브레인스토밍]]`

---

## 🌍 로어 위버 (Lore Weaver) - 세계관 설정

> 이야기가 펼쳐질 무대, 그 세계의 법칙과 비밀을 이곳에서 구축합니다.

- **[[📂 Author_Projects/Project_{{title}}/02_Lore_{{프로젝트ID}}/|➡️ 세계관 설정 폴더 바로가기]]**
- `[[📂 Author_Projects/Project_{{title}}/02_Lore_{{프로젝트ID}}/Characters_{{프로젝트ID}}/|등장인물 프로필 모음]]`
- `[[세계관_핵심_요소_{{프로젝트ID}}.md|세계관 핵심 요소]]`
- `[[주요_세력_및_조직_{{프로젝트ID}}.md|주요 세력 및 조직]]`
- `[[작품_내_주요_연표_{{프로젝트ID}}.md|작품 내 주요 연표]]`

---

## 🎭 내러티브 아키텍트 (Narrative Architect) - 플롯 설계

> 독자들을 사로잡을 매혹적인 플롯의 뼈대를 이곳에서 설계합니다.

- **[[📂 Author_Projects/Project_{{title}}/03_Narrative_{{프로젝트ID}}/|➡️ 플롯 설계 폴더 바로가기]]**
- `[[Master_Plot_Outline_{{프로젝트ID}}.md|전체 플롯 아크 개요 (200화+)]]`
- `[[Arc_01_Synopsis_{{프로젝트ID}}.md|1부 시놉시스]]` (각 부별 시놉시스 링크)
- `[[Foreshadowing_Tracker_{{프로젝트ID}}.md|떡밥 리스트 및 회수 계획]]`

---

## ✍️ 코라이팅 스튜디오 (Co-Writing Studio) - 원고 집필

> 실제 이야기가 탄생하는 공간입니다. 각 회차별 원고와 집필 관련 노트를 관리합니다.

- **[[📂 Author_Projects/Project_{{title}}/04_Manuscript_{{프로젝트ID}}/|➡️ 원고 폴더 바로가기]]**
- (Dataview 쿼리 예시: 최근 작성/수정된 원고 목록)
  ```dataview
  LIST FROM "Author_Projects/Project_{{title}}/04_Manuscript_{{프로젝트ID}}"
  WHERE contains(type, "manuscript")
  SORT file.mtime DESC
  LIMIT 5