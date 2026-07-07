# samples — 입력/산출 샘플

`instructor-support` 플러그인 스킬을 시험해 볼 수 있는 예시 자료다.

| 파일 | 역할 | 사용 스킬 |
|---|---|---|
| `course-info-sample.md` | 강의 기본정보(실제 입력) | `syllabus-design` |
| `syllabus-sample.md` | 완성된 강의계획서. 정렬 오류를 일부 심음 | `lecture-script`·`slide-outline`·`alignment-check` |

## 대표 워크플로우
1. **강의계획서 설계** — `course-info-sample.md`를 `syllabus-design`에 입력 → 강의계획서 생성
2. **정렬 점검** — 생성된 계획서(또는 `syllabus-sample.md`)를 `alignment-check`(모드A)에 입력 → ✅/⚠️/❌ 보고
3. **차시 원고** — 계획서 + "7주차"를 `lecture-script`에 입력 → 문서형 원고 + WHERETO 점검
4. **PPT 개요** — 계획서 + "3주차"를 `slide-outline`에 입력 → 슬라이드 개요 + Mayer 점검
5. (선택) 확장 — `rubric-design`·`assessment-blueprint`·`tool-mapping`

## 데모 포인트
`syllabus-sample.md`에는 의도적 정렬 오류 3개(측정 불가 동사 G5, 매핑 안 된 목표 G5, G3 분석↔중간고사 암기 불일치)가 있어, `alignment-check`가 이를 잡아내는지로 스킬 동작을 확인할 수 있다. 정답지는 파일 하단에 있다.
