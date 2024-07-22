# my-wedding
 - page : https://alicelee3.github.io/wedding/


## Project setup
> node, npm, yarn 등 사전 설치 필요
``` js
# npm install
yarn install

```

### 서버 구동
 > localhost:8080 으로 웹페이지 구동
```
# npm run serve
yarn serve
```


### 운영환경에 Deploy
> 실제로는 코드 빌드 후 docs 디렉토리 하위에 빌드 결과물을 이동시키고, 이 상태에서 remote Repo에 반영하여 Prod환경에 반영할 수 있음.
```
# npm run deploy
# 빌드 및 배포 dir에 프로젝트 코드 배포
yarn deploy

# 변경사항 수정 commit
git add .
git commit -m "수정"

# remote에 수정사항 반영
git push

# 1분 정도 기다리면 자동배포
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
