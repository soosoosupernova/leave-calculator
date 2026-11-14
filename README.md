# 연차 정산 계산기

퇴사 전에 남은 연차를 정리하는 무료 웹 계산기입니다. 회원가입·결제 없이 모든 결과가 처음부터 열립니다.

- 배포 주소: <https://soosoosupernova.github.io/leave-calculator/>
- 계산 기준: 근로기준법 제60조와 고용노동부 행정해석
- 단일 파일(`index.html`)로 동작하며 외부 의존성은 Pretendard 웹폰트와 카카오 애드핏 배너 스크립트 2건입니다.
- 결과 카드 아래에 네이버 크리에이터샵(`https://cshop.naver.com/sui_pick`) 추천 큐레이션 카드가 있습니다.
  네이버 쇼핑 커넥트 활동의 일환으로, 구매 시 일정액의 수수료를 제공받습니다.
- 입력 패널 바로 아래에 카카오 애드핏 광고단위 `DAN-DrFPkmRlhQQNbldX`(320x100)가 있습니다.
  모바일(1열)에서는 입력 폼 → 애드핏 → 결과 카드 → 큐레이션 카드 순서가 됩니다.

## 공유·검색 준비

- `og:title` / `og:description` / `og:type` / `og:url` / `og:image`(1200x630, `og-image.png`)와 `twitter:card`(summary_large_image)를 두었습니다. 카카오톡·스레드·메신저 공유 시 카드가 뜨는 부분입니다.
- `canonical`은 배포 주소를 가리킵니다.
- `sitemap.xml`과 `robots.txt`가 함께 배포됩니다. 다만 `soosoosupernova.github.io`는 GitHub Pages 공용 도메인이라 `robots.txt`는 도메인 루트에서만 읽힙니다. 실제 색인은 Google Search Console에 `sitemap.xml`을 제출하는 쪽으로 처리합니다.
- 본문 하단에 자주 묻는 질문 5개(회계연도 기준, 1년 미만 11일 정산, 14일 기한, 5인 미만, 사용촉진)와 같은 내용의 JSON-LD 구조화 데이터가 있습니다.
- `og-image.png`는 `webtools/leave-calculator/tools/make_og_image.py`로 만듭니다(페이지 기본 예시값과 같은 숫자를 사용).

## 로컬에서 열기

`index.html`을 브라우저로 열면 바로 계산됩니다. 입력값은 저장·전송되지 않습니다.
