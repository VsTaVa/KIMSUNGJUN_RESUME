<img width="1920" height="1080" alt="SAGRADAFAMILIA_김성준" src="https://github.com/user-attachments/assets/e8931cf6-2f69-4a25-854e-e6e1f45840a3" /># assets — 이미지 & 3D 자료 넣는 곳

포트폴리오에 들어갈 파일을 여기에 넣고 push 하면 Vercel이 서빙합니다.

## 폴더 구조
- `portfolio/` — 작품 이미지 (`.jpg` / `.png` / `.webp`)
  - 예: `portfolio/sagrada.jpg`, `portfolio/iron-maiden.jpg`
  - `index.html`의 포트폴리오 카드에서 `<img src="assets/portfolio/파일명.jpg">` 로 연결
- `models/` — 3D 모델 (`.glb` 권장 — 텍스처까지 한 파일)
  - 예: `models/sagrada.glb`
  - 추후 배너/포트폴리오 3D 뷰어(three.js)에서 로드
<img width="1920" height="1080" alt="SAGRADAFAMILIA_김성준" src="https://github.com/user-attachments/assets/0c42d83c-f5ab-48f5-a3a2-13f2288eb4c3" />


## 텍스트 정보(제목·연도·설명·링크)
- 노션 `[구직] → [이력서]`의 DB(프로젝트들 / 경험들 / 스킬)에서 관리하면 됩니다.
- 또는 채팅으로 알려주면 반영합니다.

## 파일 이름 규칙
- 소문자 + 하이픈: `sagrada-familia.jpg` (공백/한글 파일명은 피하기 — URL 인코딩 이슈)
