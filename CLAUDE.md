## 프로젝트 개요
- GitHub Pages + Jekyll + **Chirpy v7** (`jekyll-theme-chirpy 7.6.0`) 블로그
- 로컬 서버: `bundle exec jekyll serve --livereload` → `http://localhost:4000`
- 배포: `main` 브랜치 push → GitHub Actions 자동 빌드

## 핵심 운영 규칙
- **항상 한국어로 답변**, 코드 식별자는 그대로.
- **멋대로 수정 금지** — 묻는 말에만 대답. 코드 수정은 명시적으로 요청받은 것만.
- **최소한의 수정** — 요청 범위를 벗어난 리팩토링/개선 금지.

## 포스트 작성 양식 (Chirpy v7 프론트매터)
```yaml
---
title: "제목"
date: YYYY-MM-DD 00:00:00 +0900
categories:
  - 카테고리
tags: [태그]
description: 설명
toc: true
image:
  path: preview.webp
media_subpath: /_posts/카테고리/폴더명/
---
```
- 이미지는 각 포스트 폴더에 함께 보관, `media_subpath` 설정 후 파일명만 사용
- 미리보기 이미지: `image: path: preview.webp` (사용자가 직접 추가)

## 마크다운 규칙
- `<br>` 간격: `##` ↔ `##` 사이 2개 / `##` ↔ `###`, `###` ↔ `###` 사이 1개
- 이미지 좌측정렬 (float 없음): `{: .normal }`
- 경고 블록: `> 내용\n{: .prompt-warning }` / `{: .prompt-danger }` / `{: .prompt-info }` / `{: .prompt-tip }`
- 버튼: `[텍스트](URL){: .btn .btn--info}`

## 카테고리 구조
- `dodo` — WoW 애드온 소개 포스트
- `MDT` — 쐐기 루트 포스트

## 커스텀 파일
| 파일 | 내용 |
|---|---|
| `assets/css/jekyll-theme-chirpy.scss` | 커스텀 CSS (그리드, 색상, 사이드바 등) |
| `_layouts/default.html` | 홈 페이지 우측 패널 숨김, container/main padding 조정 |
| `_layouts/home.html` | 카드 description 제거 |
| `_config.yml` | paginate: 6 |

수정 내용 상세는 `memo.txt` 참고.

## 구형 포스트 → Chirpy 변환 시 제거 항목
`search: true`, `toc_label:`, `header: teaser:`, `last_modified_at:`, `# bundle exec jekyll serve`
