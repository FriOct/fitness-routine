# 12주 피트니스 루틴

모바일에서 보기 편한 운동 루틴 뷰어입니다.

## 파일 구조

```
fitness-routine/
├── index.html     ← 뷰어 (수정 불필요)
├── routine.json   ← 루틴 데이터 (여기만 수정)
└── README.md
```

## GitHub Pages 배포 방법

1. GitHub에서 새 레포지토리 생성 (예: `fitness-routine`)
2. 이 폴더 안의 파일 3개를 모두 업로드
3. 레포 **Settings → Pages → Source: Deploy from a branch → main → / (root) → Save**
4. 잠시 후 `https://[유저명].github.io/fitness-routine` 접속

## 루틴 수정 방법

`routine.json`만 수정하면 됩니다. HTML은 건드릴 필요 없어요.

- 운동 추가/삭제: `workouts` 배열의 `exercises` 수정
- 일정 변경: `phases` 배열의 `schedule` 수정
- 스트레칭 추가: `stretching.daily` 수정
