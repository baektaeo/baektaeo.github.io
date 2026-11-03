# Anima — OAuth 공개 안내 사이트

Google OAuth 프로덕션 앱의 브랜딩에 사용할 수 있는 **정적 안내 사이트**입니다. 실제 Anima 앱이나 개인 데이터를 공개하지 않습니다.

## 구성

- `index.html` — 앱 안내(홈페이지)
- `privacy.html` — 개인정보처리방침
- `terms.html` — 이용 안내
- `style.css` — 반응형 디자인
- `.nojekyll` — GitHub Pages 정적 파일 처리를 위한 빈 파일

## 새 GitHub 저장소에 게시

현재 계정에 Anima 전용 저장소가 없어 기존 프로젝트에 파일을 추가하지 않았습니다. 다음 순서로 게시할 수 있습니다.

1. https://github.com/new 에서 **`baektaeo.github.io`**라는 이름의 **Public** 저장소를 새로 만듭니다. 이미 이 이름을 사용하고 있다면 다른 이름으로 만들고 아래 주소를 그에 맞게 바꿉니다.
2. 이 폴더의 파일을 저장소 **최상위(root)**에 업로드합니다. ZIP 파일 자체를 올리는 것이 아니라 압축을 풀어 개별 파일을 올리십시오.
3. 저장소의 **Settings → Pages → Build and deployment**에서 `Deploy from a branch`, `main`, `/(root)`를 설정합니다.
4. 배포가 완료되면 `https://baektaeo.github.io/`와 `https://baektaeo.github.io/privacy.html`을 확인합니다.
5. Google Cloud Console → **Google Auth Platform → Branding**에서:
    - 홈페이지: `https://baektaeo.github.io/`
    - 개인정보처리방침: `https://baektaeo.github.io/privacy.html`
    - 서비스 약관(선택): `https://baektaeo.github.io/terms.html`
    - 승인된 도메인: `baektaeo.github.io` (Console이 요구하는 경우)
6. Google이 도메인 소유 확인을 요구하면 Search Console에서 사용자 소유 `baektaeo.github.io` 사이트를 확인하고, 안내되는 HTML 파일 또는 메타 태그를 사이트에 추가합니다. GitHub Pages의 공유 `github.io` 상위 도메인 전체를 소유한 것처럼 등록하지 마십시오. 별도 도메인을 요구받는 경우 소유 도메인을 연결해야 할 수 있습니다.

## 배포 전 검토

- 문의용 이메일이 **공개 게시**됩니다: `doyeon246437@gmail.com`. 필요하면 전용 지원 이메일로 변경하십시오.
- 개인정보처리방침은 2026-11-03 시점의 Anima PC·Android 구현을 기준으로 작성되었습니다. 기능 변경 시 갱신해야 합니다.
- 현재 Google Drive 동기화는 버전별 백업 파일을 남길 수 있고, 연결 해제만으로 백업을 삭제하지 않습니다. 앱 상태에 저장된 AI 제공자 API 키가 백업에 포함되는지 반드시 검토하십시오.
- 공개 페이지의 게시와 Google OAuth 검증/프로덕션 승인은 별개입니다. Google의 추가 도메인 확인 또는 인증 심사가 필요할 수 있습니다.
- 이 사이트는 자바스크립트, 외부 추적 도구, 웹폰트 요청을 사용하지 않습니다.