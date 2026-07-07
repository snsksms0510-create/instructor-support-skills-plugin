# 교수자 지원 에이전트 (Instructor Support Skills)

교수설계 근거(ABCD·Bloom·구성적 정렬·WHERETO·Mayer)에 기반해, 교수자가 강좌를 **설계하고 운영하는 전 과정**을 돕는 Claude Code 스킬 마켓플레이스입니다.

## 설치

```
/plugin marketplace add leedonwoo2827-ship-it/instructor-support-skills
/plugin install instructor-support@instructor-support-skills
```

설치 후 자연어로 요청하거나 `/syllabus-design` 처럼 스킬을 직접 호출합니다.

## 스킬 (7개)

**전체 실행** — `design-course`(전 과정 일괄 실행 오케스트레이터)

**핵심** — `syllabus-design`(강의계획서) · `lecture-script`(차시 원고) · `slide-outline`(PPT 개요) · `alignment-check`(정렬 점검)

**확장** — `rubric-design`(루브릭) · `assessment-blueprint`(평가 청사진·문항) · `tool-mapping`(도구 매핑)

## 한 번에 전체 실행

`design-course` 스킬을 호출하면 전체 파이프라인이 순서대로 실행됩니다:
강의계획서 → 정렬 점검 → 평가 설계 → 차시 원고/PPT → 도구 매핑 → 최종 점검.

- 강의 기본정보를 주거나, 완성된 강의계획서(파일 첨부)를 주거나, 아무것도 없이 호출하면 강의 정보를 되물어봅니다.
- 예: "이 강의계획서로 전체 설계해줘" + `syllabus-sample.md` 첨부

## 개별 사용

```
강의 기본정보 → syllabus-design → alignment-check → lecture-script / slide-outline
```

`samples/` 폴더의 예시로 바로 실행해 볼 수 있습니다.

## 문서
- [스킬 상세](docs/skills.md) — 입력·산출물·스킬 간 계약
- [설계 원리](docs/design-principles.md) — 정렬 규칙·프레임워크·기여 규약
- [샘플 사용법](samples/README.md)
