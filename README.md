# 프랑스어 시제 지도 (French Tense Master)

프랑스어의 시제와 법을 한 장에 정리한 지도와 연습 문제입니다.
서버나 빌드 도구 없이 `index.html` 파일 하나로 동작합니다.

**접속 주소:** https://hyungwookha.github.io/frenchtensmaster

## 구성
- **지도** (`#tense-map`): 시제·법 지도, 시제별 상세 설명, 활용표(동사 10개), 시제 일치 표, PONS 보충 설명
- **연습** (`#practice`): 활용 쓰기 / 시제 고르기(26문제) / 시제 일치(14문제)
- 오답 기록은 방문자 각자의 브라우저(localStorage `french-tenses-miss`)에만 저장됩니다.

## 고칠 때 볼 곳 (`index.html` 안)
| 이름 | 내용 |
|---|---|
| `T` | 시제별 설명 |
| `FORMS`, `AUX` | 활용형 데이터 (`conj()`가 활용형을 만듦) |
| `PONS` | PONS 보충 설명 (초록 상자) |
| `SOT` | 시제 일치 표 |
| `CHOOSE` | 「시제 고르기」 문제 (`o[0]`이 정답, 화면에서는 섞여 나옴) |
| `SOTQ` | 「시제 일치」 문제 (`o[0]`이 정답) |
| `:root` CSS 변수 | 색상 (다크 모드 포함). 우측 상단 버튼으로 고른 테마는 localStorage `french-tenses-theme`에 저장 |

## 출처
초록 상자 내용은 PONS 「Grammatik Französisch – Auf einen Blick」 2~4장의 시제 내용을 한국어로 정리한 것입니다.
