# 12주 피트니스 루틴

오늘 요일을 자동 감지해서 그날의 루틴만 보여주는 모바일 최적화 운동 앱.

## 파일 구조

```
fitness-routine/
├── index.html     ← 뷰어 (수정 불필요)
├── routine.json   ← 웨이트/스트레칭 데이터 (여기만 수정)
├── schedule.js    ← C25K 인터벌 데이터
└── README.md
```

## 기능

- 오늘 요일 자동 감지 → 해당 루틴 표시
- 운동 전 근육통 체크 → 유산소 강도 자동 조정
- C25K 트레드밀 인터벌 (주 3일: 월/수/금) 통합
- 스트레칭 영상 링크 연결
- 시작일 기준 C25K 주차 자동 계산

## 시작일 설정

`routine.json`의 `startDate`를 운동 시작 날짜로 변경하면 C25K 주차가 자동 계산돼요.

```json
"startDate": "2026-04-14"
```

## GitHub Pages 배포

1. GitHub 새 레포 생성 (public)
2. 파일 4개 업로드
3. Settings → Pages → main branch → Save
4. `https://[유저명].github.io/fitness-routine` 접속
