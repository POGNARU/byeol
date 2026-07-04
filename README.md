# 별 (byeol) — 밤하늘 서고

포근나루 / 디퍼 OS의 **밤하늘(nightsky) 아카이브**. 한 주 동안 길어 올린 씨앗·오아시스 문장이 별이 되어 뜨는 밤하늘 대시보드를 한자리에 모은다.

- **공개 링크**: https://pognaru.github.io/byeol/
- **공개 범위**: 링크 아는 사람만 (검색 차단 — 모든 페이지 `noindex` + `robots.txt Disallow /`)
- **호스팅**: GitHub Pages (POGNARU/byeol, main 브랜치)

## 구조

```
byeol/
├─ index.html          # 서고 표지 (밤하늘 갤러리)
├─ entries/            # 각 주 밤하늘 HTML
│  └─ nightsky_YYYY-MM-DD.html
├─ robots.txt          # 검색엔진 전면 차단
├─ .nojekyll           # Jekyll 처리 비활성화
└─ README.md
```

## 새 밤하늘 추가하는 법

1. 사막여우 "밤하늘" 명령으로 그 주 대시보드를 만든다 (실명은 `○○`로 가림).
2. 완성된 `nightsky_YYYY-MM-DD.html`을 `entries/`에 복사한다 (`<meta name="robots" content="noindex, nofollow">` 포함).
3. `index.html`의 `.grid` 맨 위에 카드 한 장을 추가한다 (최신이 위).
4. `git add -A && git commit && git push` — GitHub Pages가 자동 배포한다.

## 원칙

- **원본은 볼트에.** 밤하늘 원본은 `deeper-salon/00-Daily/밤하늘/`에 있고, 여기엔 실명을 가린 공개본만 둔다.
- **실명 가림.** 등장 인물 실명은 `○○`, 제목은 "나의 밤하늘". 볼트 원본 씨앗은 손대지 않는다.
