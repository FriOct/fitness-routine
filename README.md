# 12주 피트니스 루틴

[Live Demo](https://frioct.github.io/fitness-routine/)

오늘 날짜를 기준으로 루틴을 보여주고, 원하는 요일로 바로 전환해서 확인할 수 있는 모바일 최적화 운동 앱.

## 파일 구조

```
fitness-routine/
├── index.html     ← 메인 뷰어
├── routine.js     ← 앱에서 직접 로드하는 루틴 데이터
├── routine.json   ← 원본 루틴 데이터
├── schedule.js    ← C25K 인터벌 데이터
└── README.md
```

## 기능

- 오늘 날짜 기준 루틴 표시 + 다른 요일 직접 선택
- 운동 전 근육통 체크 → 유산소 강도 자동 조정
- C25K 트레드밀 인터벌 통합
- 스트레칭 영상 링크 연결
- 휴식일별 가벼운 회복 활동 표시
- 시작일 기준 C25K 주차 자동 계산

## 시작일 설정

`routine.json`의 `startDate`를 운동 시작 날짜로 변경하면 C25K 주차가 자동 계산돼요. 배포용 앱은 `routine.js`를 읽으므로 데이터 변경 후에는 `routine.js`도 함께 갱신해야 합니다.

```json
"startDate": "2026-04-14"
```

## GitHub Pages 배포

1. GitHub 새 레포 생성 (public)
2. 파일 업로드
3. Settings → Pages → main branch → Save
4. `https://[유저명].github.io/fitness-routine/` 접속
