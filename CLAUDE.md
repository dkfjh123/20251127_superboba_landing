# CLAUDE.md — 슈퍼보바 B2B 랜딩페이지

카페 사장님 대상 생보바·슈퍼호두 공급(B2B) 랜딩페이지. `index.html` 단일 파일 정적 사이트 (이미지는 Cloudflare R2 URL 참조).

## 필수 참조 문서

- [SUPERBOBA_CONTEXT.md](SUPERBOBA_CONTEXT.md) — 브랜드 **사실**(법인·매장·메뉴·가격·리뷰·컬러). 콘텐츠 작성 전 필독.
- [SUPERBOBA_MESSAGES.md](SUPERBOBA_MESSAGES.md) — **카피·문구·톤앤매너** 원천 (A 공통 진실 → B 소비자용 → C 파트너용).

## 절대 규칙

1. 🚫 **"초진주" / "超珍珠" 표기 사용 금지** (2026-07-08 확정). 법인 등기 상호를 사실 그대로 인용할 때만 예외. 브랜드 호칭은 "슈퍼보바 / SUPERBOBA"로 통일.
2. **키컬러는 슈퍼보바 레드 `#CC2222`** (hover `#9E1A1A`). 흑당 브라운 팔레트는 2026-06-08 폐기됨. 세부 팔레트·Do/Don't는 SUPERBOBA_CONTEXT.md §9.
3. 🟡 표시된 미확정 정보(영업시간, B2B 단가·MOQ·공급형태 등)는 임의로 지어내지 말 것 — 확인 후 채운다.
4. 이 랜딩의 목적은 **도입 문의 전환**. 문의 폼은 **Web3Forms**(`api.web3forms.com/submit`) → dkfjh1234@gmail.com (무료 250건/월, 대시보드 web3forms.com).
   - 🚫 formsubmit.co는 한글 전송 시 서버 500 버그로 **2026-07-09 폐기** — 되돌리지 말 것.
   - ⚠ Web3Forms에 multipart(FormData)로 보내면 **한글 필드명이 깨진다** → AJAX는 반드시 `URLSearchParams`(urlencoded)로 전송 (index.html 폼 JS에 구현됨).
5. 🚫 **"냉동" 디스 금지** (2026-07-08 확정): 슈퍼보바 B2B 공급 펄도 **냉동 유통**이다. 공격 축은 "압착 공법·수입산·평범한 식감"이지 "냉동" 자체가 아니다 — "같은 냉동이라도, 얼리기 전이 다릅니다". "냉동이 아닌~"류 카피는 직영 매장(B2C) 설명에만 허용.

## 알려진 이슈 (2026-07-09 기준)

- **배포**: GitHub main 푸시 → Cloudflare Pages 자동 배포 (`https://20251127-superboba-landing.pages.dev`). 커스텀 도메인은 미연결.
- `_*.png` 스크린샷은 확인용 임시 파일 — 커밋하지 않는다.
