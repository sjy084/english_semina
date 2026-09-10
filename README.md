# 단어장

한글 뜻을 보고 영단어를 떠올리거나 직접 입력해서 외우는 정적 사이트입니다.

## 파일
- `index.html` — 사이트 전체 (HTML/CSS/JS 하나)
- `words.json` — 단어 데이터

## 단어 추가
`words.json`에 항목을 추가하면 됩니다. `pos`는 생략해도 됩니다.

```json
{ "word": "abandon", "pos": "v.", "meaning": "버리다, 포기하다" }
```

## GitHub Pages로 올리기
1. 새 저장소를 만들고 이 세 파일을 올립니다.
2. Settings → Pages → Branch를 `main`, 폴더를 `/ (root)`로 지정합니다.
3. 1~2분 뒤 `https://<계정>.github.io/<저장소>/`에서 확인합니다.

로컬에서 바로 열면(`file://`) 브라우저가 `words.json`을 읽지 못하므로, 그 경우엔 `python3 -m http.server`로 띄우거나 GitHub Pages에서 확인하세요.

## 단축키
- `Space` 또는 `Enter` — 정답 보기 / 채점 / 다음
- `1` — 몰랐음, `2` — 알았음 (카드 모드에서 정답을 본 뒤)
- `S` — 섞기

학습 기록(알았음/몰랐음)은 브라우저에만 저장됩니다.
