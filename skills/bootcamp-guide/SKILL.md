---
name: bootcamp-guide
description: 로컬 싱크 관광 부트캠프 참가자의 진행 안내·길잡이. 참가자가 "어디서부터 시작해?", "다음 뭐 해?", "부트캠프 시작", "진행 상황 알려줘", "내 프로젝트 어디까지 했지" 라고 하거나 무엇을 할지 막막해할 때 사용한다. 현재 context.md를 읽어 지금 단계와 다음에 호출할 스킬을 안내한다. 실제 단계 작업은 각 단계 스킬(topic-select, region-context, tourapi-key, data-collect-validate, idea-sketch, prototype-build, pitch-deck-build)이 수행한다.
---

# Bootcamp Guide — 참가자 진행 길잡이

## 목적
모듈형 스킬 흐름에서 참가자가 **지금 어디쯤이고 다음에 뭘 호출해야 하는지**를 알려준다. 직접 작업은 하지 않고, 상태를 읽어 안내만 한다.

## 데이터 위치 (모든 스킬 공통)
주제카드·가이드·상태 템플릿은 **이 스킬(bootcamp-guide)의 `references/` 폴더**에 함께 설치된다: `references/cards/`, `references/guides/`, `references/_context-template.md`. 다른 스킬도 이 경로를 참조하므로 **어느 폴더에서 Codex를 켜도** 동작한다(스킬 설치 위치는 Codex가 안다). 프로젝트 폴더에서 직접 실행 중이면 `ft-skills/pipeline/cards`·`ft-skills/shared-context`를 대신 써도 된다.

## 동작
1. **`context.md` 확인** — 현재 작업 폴더(cwd)에 있는지 본다.
   - 없으면 → 이 스킬의 `references/_context-template.md`를 현재 폴더에 복사해 `context.md`를 만들고, "1단계 주제선정부터 시작"이라고 안내.
   - 있으면 → `단계`·각 섹션 채움 상태를 읽는다.
2. **다음 단계 판정** — 아래 표의 "완료 조건"을 순서대로 확인해, 처음으로 미완인 단계를 다음 할 일로 안내한다.
3. **안내 출력** — 현재까지 요약(주제·지역·단계) + "다음: `○○` 스킬을 실행하세요" + 그 스킬이 할 일 한 줄.

## 단계 지도
| 단계 | 스킬 | 완료 조건(context.md) |
|---|---|---|
| 1 | `topic-select` | `주제`가 채워짐 |
| 2 | `region-context` | `지역`이 채워짐 |
| 3 | `tourapi-key` | `TourAPI키: 등록됨/활성확인` |
| 4 | `data-collect-validate` | `데이터 검증 요약`이 채워짐 |
| 5 | `idea-sketch` | `아이디어`(사용자·시나리오·기능·MVP)가 채워짐 |
| 6 | `prototype-build` | `산출물`에 prototype.html |
| 6b | `pitch-deck-build` | `산출물`에 pitch-deck.html (+스피커노트) |
| 7~9 | Meta App | 오피스아워 예약·발표(스킬 아님) |

**선택(언제든)**: `field-research`(사용자 인터뷰·여정 매핑·유사사례)와 각 스킬의 "심화" 블록으로 깊이를 더한다. 시간이 남으면 다음으로 서두르지 말고 지금 단계를 더 파라고 안내한다.

## 안내 톤 (퍼실리테이터)
- 초보 팀 기준. 한 번에 **다음 한 단계만** 제시(전체를 쏟지 않는다).
- **팀 주도**: 정답을 주지 말고 "정답은 없다 — 데이터 보고 팀이 고른다"를 상기시킨다. 각 단계는 팀 토의로 진행된다는 걸 알려준다.
- 진행이 한 명에게 쏠려 있으면 *"다른 분들 생각은요?"* 로 참여를 넓힌다.
- 막히면 각 스킬의 "막힐 때 힌트"를 참고하라고 안내.

## 예시 출력
> 지금 상태: 주제=[N3 숙박병목], 지역=미정, 단계 1 완료.
> 다음: **`region-context`** 실행 → 후보 지역 중 1곳을 골라 컨텍스트를 잡습니다.
