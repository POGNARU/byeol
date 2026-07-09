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

## 별·별자리 디자인 (2026-07-09~)

밤하늘의 별과 별자리 규격은 볼트의 **`deeper-salon/00-Daily/밤하늘/_밤하늘_도안집.md`** 가 원본이다.

- **예쁜 별** — 4각 스파클 별 + 발광(glow) + 반짝임 애니메이션. 가장 밝은 2~3개엔 십자 빛줄기(glint). 북극성도 사각 스파클.
- **매번 다른 별자리** — 그 주의 결/상징으로 북두칠성·카시오페이아(W)·백조·오리온·왕관자리 중 하나. 늘 같은 모양이 되지 않게.
- **씨앗은 모두 하늘에** — 대표 씨앗만 별자리로 잇고, 나머지는 금빛 잔별로 곁에 함께 띄운다.
- **깊은 밤 배경** — `#04120C→#081E14→#0C2A1C`.

첫 적용: `entries/nightsky_2026-07-04.html` (북두칠성).

## 원칙

- **원본은 볼트에.** 밤하늘 원본은 `deeper-salon/00-Daily/밤하늘/`에 있고, 여기엔 실명을 가린 공개본만 둔다.
- **실명 가림.** 등장 인물 실명은 `○○`, 제목은 "나의 밤하늘". 볼트 원본 씨앗은 손대지 않는다.
