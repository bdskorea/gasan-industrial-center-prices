# 가산·구로 지식산업센터 시세 데이터 (Gasan & Guro Knowledge-Industry-Center Rent & Sale Prices)

서울 금천구 가산디지털단지와 구로디지털단지 **지식산업센터 111개 건물**의 임대·매매 시세를 건물 단위로 공개합니다.
아파트와 달리 지식산업센터는 실거래가 공개 체계가 촘촘하지 않아, 임차인도 소유자도 자기 호실이 시세 안에서 어디쯤인지 알기 어렵습니다. 이 저장소는 그 격차를 줄이기 위한 것입니다.

Building-level rent and sale price data for 111 knowledge-industry centers (지식산업센터, a Korean building type for light manufacturing and offices) in the Gasan and Guro digital complexes, Seoul.

## 데이터 파일

| 파일 | 내용 |
|---|---|
| `bds-research.csv` | 건물별 시세표 (111행). 컬럼: 건물명 · 지역 · 임대 중앙값/하위10%/상위90%/표본수 · 매매 중앙값/하위10%/상위90%/표본수 · 보유 매물 수 |
| `bds-research.json` | 위와 동일한 데이터 + 메타데이터(기준일, 단위 정의, 필드 설명, 출처 표기 예시) |

### 단위

- **임대 시세** = 전용면적 1평당 월 임대료 (만원). 보증금·관리비 제외.
- **매매 시세** = 전용면적 1평당 매매가 (만원).
- 1평 = 3.3058㎡.
- 모든 값은 **중앙값(median)** 이며, 하위 10%·상위 90% 백분위와 표본 수를 함께 제공합니다.

## 산출 방법

㈜부동산중개법인코리아가 실제로 중개·접수한 물건과 현장 확인 자료를 건물별로 집계한 값입니다.
표본 수가 적은 건물은 값의 신뢰구간이 넓으므로, 반드시 표본 수(`*_표본수` 컬럼)를 함께 보시기 바랍니다.
시세표는 **매주 갱신**되며, 이 저장소에는 **매달 갱신본을 커밋**합니다.

## 갱신 이력

각 커밋 메시지에 기준일이 표기됩니다. 최신 웹 버전은 아래에서 항상 확인할 수 있습니다.

- 시세표 웹페이지: https://bdskorea.com/research/
- 건물별 상세 페이지 (111개): https://bdskorea.com/building/
- 평형·용도별 매물 페이지: https://bdskorea.com/size/
- 원본 CSV: https://bdskorea.com/bds-research.csv
- 원본 JSON: https://bdskorea.com/bds-research.json

## 라이선스

[Creative Commons Attribution 4.0 International (CC BY 4.0)](https://creativecommons.org/licenses/by/4.0/deed.ko)

**출처를 표기하면 누구나 자유롭게 사용·재배포·가공할 수 있습니다.** 상업적 이용도 가능합니다.

출처 표기 예시:

> 부동산중개법인코리아 리서치 시세표 (https://bdskorea.com/research/, 2026년 8월 21일 기준)

Attribution example:

> BDS Korea Research Price Index (https://bdskorea.com/research/, as of 2026-08-21)

## 만든 곳

**㈜부동산중개법인코리아** — 서울 금천구 가산디지털단지 지식산업센터 전문 중개법인

- 홈페이지: https://bdskorea.com
- 주소: 서울특별시 금천구 가산디지털1로 168, 우림라이온스밸리 A동 1층 122호
- 전화: 02-2026-3000
- 이메일: bdscokorea@naver.com

데이터 오류 제보와 정정 요청을 환영합니다. Issues 또는 위 연락처로 알려 주세요.
