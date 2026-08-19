<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_BEFORE_LIGHTING_01" src="https://github.com/user-attachments/assets/c88141bc-1d5f-4a2e-aff5-a56399b45678" /># assets

포트폴리오에 들어갈 파일을 여기에 넣고 push 하면 Vercel이 서빙합니다.
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준" src="https://github.com/user-attachments/assets/eabdd0c2-7750-4bcd-a381-00f23445cbee" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_00" src="https://github.com/user-attachments/assets/2735e424-75b5-4b19-a7f1-3cd7b305ea21" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_01" src="https://github.com/user-attachments/assets/bbcd8ccc-5739-4567-bebd-cbead1fd70f0" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_02" src="https://github.com/user-attachments/assets/9d8817ff-25f1-4282-ab3b-6ab96c0c3491" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_03" src="https://github.com/user-attachments/assets/b69dd2fd-c688-4e3d-9ab4-d464fe7a778a" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_04" src="https://github.com/user-attachments/assets/86543375-6e7c-4a22-ae7d-1261fb06a3fc" /><img width="1920" height="1080" alt="IRON_MAIDEN_김성준_06" src="https://github.com/user-attachments/assets/beed77da-0b7b-4414-b1be-02990a3a7fb8" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_05" src="https://github.com/user-attachments/assets/69e796a3-8eb4-488d-b068-de75d3029ff8" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_06" src="https://github.com/user-attachments/assets/1320bd31-db7a-47e8-a117-4a22863fbd88" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_07" src="https://github.com/user-attachments/assets/517d7830-71f9-4894-9799-eda9f850b313" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_08" src="https://github.com/user-attachments/assets/fb26d520-97d3-4f8e-939c-cff63c773cdb" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_BEFORE_LIGHTING_01" src="https://github.com/user-attachments/assets/4745ca30-e8b0-48ed-bffe-793cd0fa4e96" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_BEFORE_LIGHTING_02" src="https://github.com/user-attachments/assets/e5faedf9-248e-4e9c-b2e4-b3ec234e67f3" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_BEFORE_LIGHTING_03" src="https://github.com/user-attachments/assets/a3273b00-79df-4f7a-a11b-eb64c04ed6bf" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_PROP" src="https://github.com/user-attachments/assets/013acf60-d426-4062-a187-9182df85b810" />
<img width="1920" height="1080" alt="IRON_MAIDEN_김성준_WIRE" src="https://github.com/user-attachments/assets/7cb66715-6daf-4353-b3d7-721622a47c30" />

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
