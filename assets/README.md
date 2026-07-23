# assets

포트폴리오에 들어갈 파일을 여기에 넣고 push 하면 Vercel이 서빙합니다.

## 폴더 구조

- `portfolio/` — 작품 이미지 (`.jpg`)
- `models/` — 3D 모델 (`.glb` 권장 — 텍스처까지 한 파일)
- `profile.jpg` — 히어로 프로필 사진
- `vstava-logo.png` — 레일 상단 로고

## 파일 이름 규칙

`{작품}-{역할}.jpg` — 소문자 + 하이픈만. 공백·한글·대문자는 URL 인코딩 문제가 생기니 피합니다.

| 역할 | 이름 | 설명 |
|---|---|---|
| 대표 | `-main` | 카드 썸네일로 쓰이는 대표 컷 |
| 타이틀 | `-00` | 타이틀/표지 이미지 |
| 렌더 | `-01` ~ `-NN` | 본편 렌더 컷 (번호 오름차순) |
| 라이팅 전 | `-before` / `-before-NN` | 라이팅 세팅 전 비교 컷 |
| 4면도 | `-ortho`, `-ortho-before` | 정면·측면·후면 4방향 뷰 |
| 와이어 | `-wire` | 와이어프레임 시트 |
| 프랍 | `-prop` | 프랍/모듈 시트 |

## 모달 표시 순서

`index.html` 하단 `projects` 객체의 `images` 배열 순서대로 표시됩니다. 세 작품 모두 아래 순서로 통일돼 있습니다.

```
main → (영상) → 00 → 렌더 오름차순 → ortho/before → wire → prop
```

영상을 끼우려면 배열에 문자열 대신 `{video:"유튜브ID"}` 를 넣습니다.

## 현재 수록 현황

| 작품 | 장수 | 파일 |
|---|---|---|
| Sagrada Familia | 16 | `sagrada-main`, `sagrada-00`~`10`, `sagrada-ortho-before`, `sagrada-ortho`, `sagrada-wire`, `sagrada-prop` |
| Iron Maiden | 12 | `iron-main`, `iron-00`~`05`, `iron-before-01`~`03`, `iron-wire`, `iron-prop` |
| M.O.L. | 13 | `mol-blue-main`, `mol-blue-00`~`04`, `mol-blue-wire`, `mol-blue-prop`, `mol-orange-01`~`03`, `mol-orange-wire`, `mol-orange-prop` |

카드 캡션의 "이미지 N장" 표기도 함께 맞춰야 합니다.

## 텍스트 정보(제목·연도·설명·링크)

노션 `[구직] → [이력서]` 의 DB(프로젝트들 / 경험들 / 스킬)에서 관리합니다.
