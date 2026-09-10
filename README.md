# 말씀 암송 · Hannah

단일 HTML 파일(`index.html`)로 동작하는 성경 구절 암송 앱입니다.
빌드 도구 없이 브라우저에서 바로 열리며, 진행 기록은 기기의 localStorage에 저장됩니다.

## 실시간 반영 (GitHub Pages)

`index.html`을 수정해서 푸시하면 GitHub Actions가 자동으로 GitHub Pages에 배포합니다.

### 최초 1회 설정

1. 저장소 **Settings → Pages** 로 이동
2. **Build and deployment → Source** 를 **GitHub Actions** 로 선택
3. 저장 후 아무 커밋이나 푸시하면 (또는 Actions 탭에서 `Deploy to GitHub Pages` 를 수동 실행) 배포됩니다.

배포 주소: https://sroyal6004-bit.github.io/memoriseword/

### 이후 수정 흐름

1. `index.html` 수정
2. 커밋 후 푸시 (`main` 또는 `claude/*` 브랜치)
3. 약 1분 뒤 위 주소에 반영 (브라우저 캐시 때문에 최대 10분 정도 걸릴 수 있음 → 새로고침)

## 파일 구조

- `index.html` — 앱 전체 (HTML + CSS + JS)
- `.github/workflows/pages.yml` — GitHub Pages 자동 배포 워크플로우
