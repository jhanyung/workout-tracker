# 12주 운동 트래커 (GitHub Pages 단일 페이지 빌드)

이 저장소는 **빌드 도구 없는** 단일 HTML 기반 PWA입니다. React/Recharts/Tailwind를 CDN으로 불러오며, 기록은 `localStorage`에 저장됩니다.

## 사용 방법

1. GitHub에서 **새 리포지토리**를 만듭니다. (예: `workout-tracker`)
2. 이 폴더의 모든 파일을 업로드합니다. (`index.html`, `manifest.webmanifest`, `sw.js`, `assets/*`)
3. 리포지토리 **Settings → Pages** 로 이동하여:
   - **Build and deployment**: `Deploy from a branch`
   - **Branch**: `main` / `/ (root)` 선택 후 저장
4. 페이지가 활성화되면 제공된 URL(예: `https://<username>.github.io/workout-tracker/`)로 접속합니다.
5. 모바일 크롬에서 **⋮ → 홈 화면에 추가** 또는 **설치** 버튼으로 PWA처럼 설치하세요.

## 개발 메모
- React/ReactDOM/Recharts는 UMD CDN을 사용, JSX는 Babel Standalone이 런타임 트랜스파일합니다(간편성 우선).
- 아이콘은 `assets/icon-192.png`, `assets/icon-512.png`를 사용합니다.
- 오프라인 캐시는 `sw.js`에서 관리합니다(간단한 캐시 전략).
- 데이터는 브라우저 `localStorage` 키 `workout_tracker_v1`에 저장됩니다.

> 필요 시 정적 번들(빌드 파이프라인) 버전도 구성해 드릴 수 있습니다.
