# nopen v0.42 — 배포 방법

## 파일 구성
- `index.html` — 앱 전체 (데이터 6,106문항·사운드·이미지 내장, 오프라인 동작)
- `sw.js` — 서비스워커 (오프라인 캐시, 캐시명 `nopen-v042`)
- `icon.png` — 홈 화면 아이콘 (180×180)

## GitHub Pages 배포 (suhumsang 계정 · 저장소 이름 nopen)
1. github.com → New repository → 이름 nopen (Public) → 이 zip의 index.html, sw.js, icon.png 업로드\n   (이미 만들었으면 기존 파일을 교체)
2. 커밋하면 1~2분 뒤 `https://suhumsang.github.io/nopen/` 에 반영
3. 아이폰 사파리에서 접속 → 공유 → **홈 화면에 추가**

## 업데이트가 반영 안 될 때
- sw.js의 캐시명이 바뀌어야 폰이 새 버전을 받는다 (이번: `nopen-v042`)
- 그래도 안 되면: 사파리에서 새로고침 2회, 또는 홈 화면 아이콘 삭제 후 재추가

## 비공개 수준
- 앱과 robots.txt에 검색엔진 차단(noindex)이 들어 있어 검색으로는 노출되지 않는다.
- 단, 무료 GitHub Pages 특성상 저장소·URL 자체는 공개다. URL을 아는 사람만 접근 가능한 수준.
- robots.txt도 저장소에 같이 업로드할 것.

## 주의
- 진행 기록·오답 노트는 폰의 localStorage에 저장 — 앱 삭제 전 **백업 내보내기**(회차 선택 화면 하단) 권장
- iOS 무음 스위치가 켜져 있으면 소리는 나지 않는다 (우회 불가)
