# RA_workshop

## 구성
- `index.html`: PDF 슬라이드 전용 뷰어
- `assets/RC_Community_Standards.pdf`: 첨부한 PDF 원본 복사본

## 실행 방법
1. `c:\coding\RA_workshop` 폴더에서 로컬 정적 서버 실행
2. 브라우저에서 생성된 주소 열기

```bash
cd c:\coding\RA_workshop
python -m http.server 8080
```

http://localhost:8080 에서 파일을 열고 좌우 화살표/버튼/터치 스와이프로 페이지 이동 가능합니다.

## GitHub 레포지토리 생성(선택)
원격 저장소를 만들려면 로컬 저장소를 먼저 초기화한 뒤 GitHub CLI 또는 기존 Git remote를 사용하세요.

```bash
git init
git add .
git commit -m "init: RA_workshop PDF slide viewer"
gh auth login
gh repo create RA_workshop --public --source=. --remote=origin --push
```
