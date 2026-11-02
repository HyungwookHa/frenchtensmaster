# 프랑스어 시제 지도 (French Tense Master)

프랑스어의 시제·법, 대명사, 관계사를 한 장씩 정리한 지도입니다.
서버나 빌드 도구 없이 HTML 파일만으로 동작합니다.

**접속 주소:** https://hyungwookha.github.io/frenchtensmaster

## 구성
- 맨 위 주제 탭 3개 (프랑스 국기 색 파랑·흰색·빨강): 시제·법 / 대명사 / 관계사
- **시제·법** (`index.html`): 시제·법 지도, 시제별 상세 설명, 활용표(동사 10개), 시제 일치 표, PONS 보충 설명
- **대명사** (`pronoms.html`): 목적보어 대명사 순서 삼각형, 대명사별·조합별 설명, 위치·일치·강세형 규칙, PONS 6장 정리
- **관계사** (`relatifs.html`): 역할 × 선행사(사람·동물/사물·중성) 관계사 표(Delatour p.211의 틀). 칸을 누르면 3단계 설명(빈자리 → 조각 → 합친 문장)과 Delatour 상자가 바뀜. 관계절의 법·일치·강조 구문 등 규칙
- 다크 모드: 우측 상단 버튼. 고른 테마는 localStorage `french-tenses-theme`에 저장되고, 주제 탭 링크에도 `?theme=`로 실려 페이지를 옮겨도 유지됩니다.

## 고칠 때 볼 곳

`index.html` 안:
| 이름 | 내용 |
|---|---|
| `T` | 시제별 설명 |
| `FORMS`, `AUX` | 활용형 데이터 (`conj()`가 활용형을 만듦) |
| `PONS` | PONS 보충 설명 (초록 상자) |
| `DELA`, `DELA_SOT` | Delatour 문법서 보충 설명 (붉은 상자 `#7F2425`, 블록마다 인쇄 쪽 번호). `delatour-tense-notes.json`에서 만든 데이터 |
| `SOT` | 시제 일치 표 |
| `:root` CSS 변수 | 색상 (다크 모드 포함, 국기 색 `--fr-bleu` `--fr-blanc` `--fr-rouge`) |

`pronoms.html` 안:

| 이름 | 내용 |
|---|---|
| `PR` | 대명사별 설명과 예문 |
| `COLS` | 삼각형 칸(①~⑤)에 들어가는 대명사 |
| `PAIR` | 두 칸을 함께 쓸 때의 판정(쓸 수 있음·드묾·못 씀)과 예문 |

`relatifs.html` 안:

| 이름 | 내용 |
|---|---|
| `C` | 표의 칸(역할-선행사)마다 관계사, 연결할 Delatour 항목, 3단계 예문 |
| `DELA` | 관계사별 Delatour 설명 (`delatour-relatives-notes.json`에서 만든 데이터) |
| `RULES` | 표 아래 규칙 상자 (Delatour·PONS) |

## 출처
초록 상자 내용은 PONS 「Grammatik Französisch – Auf einen Blick」 2~4장(시제)과 6장(대명사) 내용을 한국어로 정리한 것입니다. 대명사 페이지의 나머지 설명과 예문은 일반 문법을 바탕으로 썼습니다.

붉은 상자 내용은 Yvonne Delatour et al., *Nouvelle grammaire du français* (Paris: Hachette Français Langue Étrangère, 2004), ISBN 978-2-01-155846-6의 해당 쪽을 한국어로 정리한 것입니다. 쪽 번호는 책에 인쇄된 번호입니다.
