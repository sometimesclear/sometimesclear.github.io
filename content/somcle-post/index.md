---
emoji: 💪
title: 개츠비 블로그 만들기
date: '2023-01-18 23:11:00'
author: 썸클
tags:
categories: 개발로그
---

## 👋 소개

안녕하세요. 썸클입니다. 구직활동을 위해 블로그를 만들어보았습니다.
개발환경이 윈도우에 yarn을 주로 쓰는 덕에 조금 헤멨지만 성공했네요.
자세한 설명의 줌코딩님께 감사드립니다. 댓글의 제보와 해결방법도 도움이 많이 되었습니다.<br/><br/> [쉽고 빠르게 나만의 개츠비(Gatsby) 블로그 만들기](https://www.zoomkoding.com/gatsby-starter-zoomkoding-introduction/) 를 참고하였고 5. 블로그 배포하기에서 에러가 많이 발생했는데 하나는 댓글에 있었던 webpack 오류였습니다.<br/><br/>
해결방법은 아래와 같습니다.<br/><br/>
npm을 사용하시는 경우

```bash
npm install --save-dev "@emotion/react"
```

yarn을 사용하시는 경우

```bash
yarn add @emotion/styled
```

위와 같이 빠진 웹팩을 모두 설치해주시고

```bash
yarn run deploy
```

해주시면 됩니다.

### 윈도우에서 node 버전 변경하는 법

윈도우에서는 맥에서 쓰는 n을 쓸 수 없다고 하여 nvm을 설치했습니다.
[nvm 설치 페이지](https://github.com/coreybutler/nvm-windows/releases) 로 가서 Download now! 를 클릭하고 나오는 페이지의 Asset > nvm-setup.exe를 설치하시면 됩니다.
파워셀이나 터미널에서 아래 명령어로 설치를 확인합니다.

```bash
nvm version
```

설치된 node.js를 확인합니다.

```bash
nvm list
```

nvm으로 설치할수 있는 node.js를 확인합니다.

```bash
nvm list available
```

필요한 버전의 노드를 설치합니다.

```bash
nvm install 18.1.0
```

노드 버전을 변경합니다.

```bash
nvm use 16.15.0
```

### 🏃‍♀️ 실행하기

아래 명령어를 실행하여 로컬 환경에 블로그를 실행합니다.
npm이나 yarn 둘 중 하나만 사용하시면 됩니다.

```bash
# Install dependencies
$ npm install
$ yarn install

# Start development server
$ npm start
$ yarn start
```

<br/>

위 명령어가 문제 없이 실행됐다면 [http://localhost:8000](http://localhost:8000)에서 블로그를 확인하실 수 있습니다.

<br/>
여기까지는 되었고 내일부터 본격적으로 블로그를 다듬어봐야겠습니다.

```toc

```
