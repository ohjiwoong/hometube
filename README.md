# 홈트 루틴 플레이어

유튜브 운동 영상의 원하는 구간만 골라 이어 붙이고, 세트 반복·휴식 타이머까지 자동으로 진행하는 웹앱.

- 여러 영상 구간을 하나의 루틴으로 연속 재생, 세트·휴식 자동 진행
- 보조 화면(음악·타이머 등) 동시 재생, 거울 모드, 속도 조절
- 유튜브 검색, 영상 챕터로 구간 자동 분할 (YouTube Data API)
- 루틴 저장·공유 링크, PWA 설치, 안드로이드 공유 대상

## 로컬 실행

```
cp config.example.js config.js   # API 키 입력 (선택)
python -m http.server 5173
```

## 배포

`main`에 푸시하면 GitHub Actions가 GitHub Pages로 배포한다. API 키는 저장소 Secret `YT_API_KEY`에서 읽어 배포 시 `config.js`로 생성한다.
