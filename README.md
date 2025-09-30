# 12주 운동 트래커 (GitHub Pages 단일 페이지 빌드 - FIXED)
- `index.html`: `<script type="text/babel" data-presets="env,react">` 적용 (JSX 런타임 오류 해결)
- `sw.js`: `workout-tracker-v2`로 캐시 버전 업 (초기 오류 캐시 무효화)

## 배포
1) 리포 루트에 업로드 → 커밋  
2) Settings → Pages → `Deploy from a branch` (`main` / `/ (root)`)  
3) 휴대폰에서 접속 후 크롬 **⋮ → 홈 화면에 추가** 또는 **설치**

## 캐시 문제 시
- 새로 푸시 후, 브라우저에서 **사이트 데이터 삭제** 또는 **강력 새로고침**을 실행
