# Anima — OAuth 안내 사이트

Google OAuth 동의 화면의 브랜딩 정보 확인을 위한 **정적 안내 사이트**입니다. Anima 앱 본체와 개인 데이터는 이 저장소에 공개하지 않습니다.

## 공개 페이지

- 홈페이지: https://baektaeo.github.io/
- 개인정보처리방침: https://baektaeo.github.io/privacy.html
- 이용 안내: https://baektaeo.github.io/terms.html

## 파일

- `index.html`: 앱 목적과 주요 기능, Google Drive 연동 설명
- `privacy.html`: Google 사용자 데이터의 수집·이용·저장·공유·삭제 및 외부 API 사용 관련 개인정보처리방침
- `terms.html`: 개인용 앱 이용 안내
- `style.css`: 반응형 스타일
- `.nojekyll`: GitHub Pages 정적 파일 배포

## Google Cloud OAuth 설정

Google Cloud Console → Google Auth Platform → Branding에서 다음을 입력합니다.

- 앱 이름: **Anima**
- 애플리케이션 홈페이지: `https://baektaeo.github.io/`
- 개인정보처리방침: `https://baektaeo.github.io/privacy.html`
- 서비스 약관(필요하면): `https://baektaeo.github.io/terms.html`

Google에서 홈페이지의 도메인 소유 확인을 요구하는 경우 [Google Search Console](https://search.google.com/search-console)에서 **URL 접두어** 방식으로 `https://baektaeo.github.io/`를 추가한 후 인증합니다. HTML 메타 태그 또는 HTML 인증 파일을 제공받으면 이 저장소에 추가할 수 있습니다. 소유권 확인 후 Google Cloud 재검증에는 반영 시간이 필요할 수 있습니다.

## 데이터 처리 및 유지보수

- 이 저장소에는 Google OAuth 클라이언트 보안 비밀, 액세스 토큰, 개인 대화 데이터, API 키를 커밋하지 않습니다.
- Google Drive 동기화는 앱 전용 `drive.appdata` 범위를 사용하고, 백업 데이터는 사용자의 Google Drive에 저장됩니다.
- 동기화된 백업은 로그아웃만으로 삭제되지 않으며, 버전별 파일이 남을 수 있습니다.
- 이 사이트의 문의용 이메일 주소는 **공개**됩니다. 지원용 이메일을 변경할 경우 세 HTML 파일의 연락처도 수정해야 합니다.
- 이 문서는 2026년 11월 현재 확인한 Anima 구현을 기준으로 작성되었으며, 기능 변경 시 개인정보처리방침을 업데이트해야 합니다.
