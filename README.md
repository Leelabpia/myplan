# 나만의 HQ

> 오늘의 일과 / 업무계획(날짜범위) / 했던 일 대시보드 - 나만 쓰는 Private 앱

## 📂 파일
- `index.html` : 앱 전체 (단일 파일, 그대로 배포)
- `manifest.json` : PWA 앱 정보 (홈화면 설치용)
- `sw.js` : 오프라인 캐시용 서비스워커

## 🚀 GitHub Pages 배포 (가장 쉬운 방법)

1. **리포 생성**
   - github.com → New repository → 이름 `my-hq` → Public → Create

2. **파일 업로드**
   - `Add file > Upload files` → `index.html`, `manifest.json`, `sw.js` 3개 업로드 → Commit

3. **Pages 켜기**
   - Settings → Pages → 
   - Source: `Deploy from a branch`
   - Branch: `main` / `/(root)` → Save
   - 1~2분 뒤 상단에 `https://USERNAME.github.io/my-hq/` 주소 생김

4. **휴대폰에 앱처럼 설치**
   - iPhone: Safari로 접속 → 공유 → 홈 화면에 추가
   - Android: Chrome으로 접속 → ⋮ → 홈 화면에 추가 / 앱 설치

데이터는 폰 브라우저의 localStorage에 저장됩니다. 다른 사람이 접속해도 각자 폰에만 저장되어 완전히 분리됩니다.

## 💾 Google Drive 백업
앱 상단의 `드라이브에 저장` / `드라이브에서 불러오기` 버튼으로 JSON 백업/복원 가능.
Google Drive API 연동 원하면 `gdrive.js` 추가 예정.

## 🛠 수정 방법
`index.html` 하나만 수정하면 됩니다. React 빌드 필요 없이 바로 반영됩니다.

## 📱 PWA 기능
- 홈 화면 아이콘
- 전체화면 standalone 실행
- 오프라인에서도 열림
