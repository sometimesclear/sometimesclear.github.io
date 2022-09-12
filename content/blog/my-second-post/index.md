---
title: 블로그 개설!
date: "2022-09-12T15:26:37.121Z"
---

드디어 블로그 만들었다. Gatsby를 썼습니다.

## Gatsby란?

> 정적 사이트 생성기. 리액트 기반 오픈소스 프레임워크.
> 개인 포트폴리오나 블로그 만들 때 유용함.

gatsby 블로그 만드는 것 자체는 어렵지 않았는데 git 연동이 안되어서 해결하느라 애먹었다.

1. [gatsbystarter](https://www.gatsbyjs.com/starters/)에서 원하는 템플릿을 정한다. 나는 gatsby-starter-blog 로 정했다.
2. ```
   npx gatsby new gatsby-starter-blog https://github.com/gatsbyjs/gatsby-starter-blog
   ```

설치하면 gatsby-starter-blog 폴더가 생긴다. 터미널에 `cd gatsby-starter-blog` 를 쳐서 해당 폴더로 이동한다.

3. 아래 명령어로 원격 저장소로 푸시. (여기서 에러가 발생했다.)

```
git add.
git commit -m 'commit test'
git remote add origin https://github.com/깃허브아이디/저장소이름.git
git push -u origin master

```

4. github에 저장소를 만든다. 추후 배포를 위해 원하는이름.github.io 로 생성한다.

### 에러 상황

1. git push가 안됨. `error: src refoes not match` 라고 한다.

   - 검색해보니 원격 저장소에서 pull 을 받지 않고 로컬 저장소에서 push를 했을 때 생기는 에러라고 한다. 아래와 같이 초기화하여 다시 진행.

   ```
   git init // 깃 초기화
   git add .
   git commit -m 'message'
   git remote add origin 'github.com/저장소이름.git'
   git push -u origin master

   ```

   그래도 안되어서 확인해보니 내 로컬 브랜치 이름이 main 이 아닌 master였는데 내가 계속 main으로 푸시를 해서 그런 것 같다.
