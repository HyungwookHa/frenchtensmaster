# 작업 규칙 (Claude용)

이 저장소는 HTML 파일로 동작하는 「프랑스어 학습 지도 (시제-대명사-관계사)」입니다. `index.html`(시제·법), `pronoms.html`(대명사), `relatifs.html`(관계사)이 있고, 맨 위 국기 색 탭으로 오갑니다. 사이트: https://hyungwookha.github.io/lestempslespronomslesrelatifs
코드 구조는 `README.md`의 「고칠 때 볼 곳」 표를 참고하세요.

## 반드시 지킬 작업 순서
1. 사용자가 수정 사항을 말하면 `index.html`, `pronoms.html`, `relatifs.html`(필요하면 `README.md`도)을 고친다.
2. **push하기 전에** Artifact 도구로 미리보기 링크를 준다. `index.html`을 페이지로, `files`에 `{"pronoms.html": "pronoms.html", "relatifs.html": "relatifs.html", "coq.png": "coq.png"}`을 함께 게시한다 (`coq.png`는 국기 탭 위 수탉 그림).
   - 같은 대화에서 다시 고칠 때는 같은 파일 경로로 다시 게시해서 링크를 유지한다.
   - 무엇이 바뀌었고 어디를 눌러 확인하면 되는지 짧게 알려준다.
3. 사용자가 미리보기를 보고 추가로 지시하면 2번을 반복한다.
4. 사용자가 올리라고 **명시적으로 허락한 뒤에만** 커밋하고 push하고 `main`으로 PR을 만든다.
   - PR을 만든 뒤에는 PR 화면에서 Merge 버튼을 누르면 사이트에 반영된다고 안내한다.

## 기타
- 사이트는 정보 전달이 목적이다. 연습 문제는 넣지 않는다.
- 문법 보충 상자: 초록 = PONS 문법표, 붉은색 `#7F2425` = Delatour 『Nouvelle grammaire du français』. Delatour 내용은 블록마다 인쇄 쪽 번호로 출처를 단다.
- 사용자는 주로 안드로이드 휴대폰으로 작업한다. 휴대폰 화면 폭(약 390px)에서도 잘 보이는지 확인한다.
- 답변은 한국어로, 쉬운 말로 한다.
