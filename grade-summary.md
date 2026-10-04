# 숭실대학교 2026학년도 국제저명논문 등급 분류 정리

> 원본: 『숭실대학교 2026학년도 국제저명논문 등급 분류.xlsx』
> 검색 사이트: <https://baelab-create.github.io/ssu-journal-grade-2026/>
> 정리일: 2026.09.18

---

## 1. 등급 체계 요약

| 등급 | 대상 | 산정 기준 |
|---|---|---|
| **S** | SCIE·SSCI 등재지 최상위 | JCR 랭킹 IF 기준 |
| **A** | SCIE·SSCI 상위 + **A&HCI 등재지 전체** | JCR 랭킹 IF 기준 (A&HCI는 일괄 A등급 인정) |
| **B** | SCIE·SSCI 중위 | JCR 랭킹 IF 기준 |
| **C** | SCIE·SSCI 하위 | JCR 랭킹 IF 기준 |
| **D** | **SCOPUS 전용 등재지** | SCIE·SSCI·A&HCI 미등재 + SCOPUS 등재 |

### 핵심 규칙

- **SCIE·SSCI**: JCR 랭킹 IF를 기준으로 등급 산정.
- **복수 카테고리 저널**: 2개 이상의 카테고리에 동시에 속하는 경우, **가장 유리한 카테고리의 등급을 적용**(조정등급 우선 적용). 예: 한 저널이 ECONOMICS에서 A, ENVIRONMENTAL STUDIES에서 B라면 → 조정등급 A 인정.
- **A&HCI**: 등재지 전체를 국제저명 **A등급**으로 인정.
- **SCOPUS**: SCIE·SSCI·A&HCI와 중복되지 않는 등재지를 **D등급**으로 인정. Inactive 저널 및 ScopusID 미부여 저널은 제외.
  - ※ 실제 데이터에는 SCIE/SSCI 등재지가 SCOPUS 시트에도 중복 수록된 사례가 존재(예: Energy Economics). 이 경우 상위 등급(SCIE/SSCI 기준)이 적용됨.

---

## 2. 데이터 규모 (원본 엑셀 기준)

| 시트 | 행 수(저널×카테고리) | 비고 |
|---|--:|---|
| SCIE | 15,043 | 2024 JCR 기준 |
| SSCI | 5,029 | 2024 JCR 기준 |
| A&HCI | 1,980 | 전체 A등급 |
| SCOPUS(국제D) | 30,294 | 전체 D등급 |
| **합계** | **52,346** | |

※ 행 수는 "저널 × 카테고리" 단위. 한 저널이 여러 카테고리에 속하면 여러 행으로 수록됨.

### 등급 분포 (시트별 행 기준)

| 시트 | S | A | B | C | D |
|---|--:|--:|--:|--:|--:|
| SCIE | 951 | 3,590 | 4,238 | 6,264 | – |
| SSCI | 439 | 1,534 | 1,511 | 1,545 | – |
| A&HCI | – | 1,980 | – | – | – |
| SCOPUS | – | – | – | – | 30,294 |

### 조정등급 분포 (복수 카테고리 유리 등급 적용 후)

| 구분 | S | A | B | C |
|---|--:|--:|--:|--:|
| SCIE (SCI_x) | 1,280 | 4,168 | 4,380 | 5,212 |
| SSCI (SSCI_x) | 593 | 1,756 | 1,486 | 1,194 |

※ 조정등급이 카테고리별 등급보다 많은 이유: 유리한 등급이 저널의 모든 카테고리 행에 적용되기 때문.

---

## 3. 주요 컬럼 설명 (SCIE/SSCI 시트)

| 컬럼 | 의미 |
|---|---|
| Journal Title / Title Abbr | 학술지명 / 약칭 |
| ISSN / E_ISSN | 인쇄판 / 온라인판 ISSN |
| 등급 | 해당 카테고리에서의 등급 (S/A/B/C) |
| 조정등급 | 복수 카테고리 중 가장 유리한 등급 (SCI_S, SSCI_A 등) — **실제 인정 등급** |
| Category Description | JCR 카테고리 |
| IF / IF(%) | Impact Factor / 카테고리 내 IF 상위 백분율 |
| Rating / Rank | Quartile(Q1~Q4) / 카테고리 내 순위 |

---

## 4. 연구실 관련 학술지 등급 예시 (BAE LAB 투고 실적 기준)

| 학술지 | 등재 | 등급 | 비고 |
|---|---|---|---|
| Biomimetics | SCIE + SCOPUS | **A** (SCI_A) | ENGINEERING, MULTIDISCIPLINARY Q1 |
| Electronics | SCIE + SCOPUS | **B** (SCI_B) | ENGINEERING, ELECTRICAL & ELECTRONIC Q2 |
| J. of Electrical Engineering & Technology (JEET) | SCIE + SCOPUS | **C** (SCI_C) | |
| Polymer(Korea) | SCIE + SCOPUS | **C** (SCI_C) | 국내 발행 SCIE지 |
| World Patent Information | SCOPUS | **D** | 특허 분야 전문지 |
| Foresight (Emerald) | SCOPUS | **D** | 미래예측·기술경영 |
| 전기학회논문지 (Trans. KIEE) | SCOPUS | **D** | 국내지이나 SCOPUS 등재 |
| 한국산학기술학회논문지 | KCI 전용 | 등급 없음 | 국제저명 DB 미등재 |

---

## 5. 유의사항

- 본 정리는 참고용이며, **최종 등급은 학교 공식 자료를 기준**으로 확인할 것.
- 등급은 학년도별로 갱신되므로 2027학년도 분류 발표 시 재확인 필요.
- 학술지명·ISSN으로 바로 검색: <https://baelab-create.github.io/ssu-journal-grade-2026/> (분야별 탐색·등급 필터 지원)
