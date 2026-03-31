# Golden Record Landing

`index.html`을 GitHub에 올린 뒤 Railway에 바로 배포할 수 있도록 최소 서버 구성을 추가한 프로젝트입니다.

## 로컬 실행

```bash
npm start
```

브라우저에서 `http://localhost:3000`으로 확인할 수 있습니다.

## GitHub 업로드

```bash
git init
git add .
git commit -m "Initial deployable landing page"
git branch -M main
git remote add origin <YOUR_GITHUB_REPO_URL>
git push -u origin main
```

## Railway 배포

1. Railway에서 `New Project`를 누릅니다.
2. GitHub 저장소를 연결합니다.
3. 배포가 시작되면 Railway가 `npm start`로 서버를 실행합니다.
4. 배포 후 발급된 도메인으로 접속합니다.

`server.js`는 Railway가 주입하는 `PORT` 환경변수를 사용합니다.
