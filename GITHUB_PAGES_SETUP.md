# GitHub Pages 배포 가이드

## 1단계: GitHub에서 새 저장소 생성

1. https://github.com/new 방문
2. 저장소 이름 입력 (예: `kcsat-leaderboard`)
3. **Public** 선택 (GitHub Pages는 Public 저장소에서 무료)
4. **"Initialize this repository with a README" 체크 해제** (이미 파일이 있으므로)
5. "Create repository" 클릭

## 2단계: 로컬 저장소를 GitHub에 푸시

GitHub에서 제공하는 명령어를 사용하거나, 아래 명령어를 실행하세요:

```bash
cd /Users/inbum/workspace/isoft_KCSAT_LeaderBoard

# GitHub 저장소 URL을 YOUR_USERNAME과 YOUR_REPO_NAME으로 변경하세요
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

예시:
```bash
git remote add origin https://github.com/inbum/kcsat-leaderboard.git
git branch -M main
git push -u origin main
```

## 3단계: GitHub Pages 활성화

1. GitHub 저장소 페이지로 이동
2. **Settings** 탭 클릭
3. 왼쪽 메뉴에서 **Pages** 클릭
4. **Source** 섹션에서:
   - Branch: `main` 선택
   - Folder: `/ (root)` 선택
5. **Save** 클릭

## 4단계: 배포 완료!

몇 분 후 다음 URL로 접속 가능합니다:
- `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

예시:
- `https://inbum.github.io/kcsat-leaderboard/`

**참고:** 
- 첫 배포는 1-2분 정도 걸릴 수 있습니다
- `index.html`이 루트에 있으면 자동으로 표시됩니다
- `index_server.html`로 접근하려면 `/index_server.html`을 URL에 추가하세요

