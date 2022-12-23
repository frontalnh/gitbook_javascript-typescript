# Managing Packages



`yarn.lock`  에 있는 대로 `yarn install` 을 하면 설치될 것 같지만, 기본적으로 `yarn install` 은 `package.json` 과 `yarn.lock` 이 다르면 `package.json` 에 있는대로 `yarn.lock` 을 업데이트 한다.



따라서 정확히 `yarn.lock` 에 있는 대로 패키지를 설치하고자 한다면 아래와 같이 `--frozen-lockfile` 옵션을 함께 사용해 주는것이 안전하다.



```
yarn --frozen-lockfile
```
