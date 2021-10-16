# svelte app

## 배포된 사이트 확인하기

https://hello-svelte-eight.vercel.app/

## Svelte 프로젝트 시작하기

프로젝트 시작 템플릿 받아오기

```bash
npx degit sveltejs/template 폴더이름
cd 폴더이름
```

## 설치 및 개발 준비

필요한 패키지들 설치하기

```bash
cd 폴더이름
npm install
```

package.json에 있는 dev script 실행하기

```bash
npm run dev
```

실행한 후 크롬으로 이 링크 들어가기 [localhost:5000](http://localhost:5000).

끄고 싶을 때는 `ctrl + c` 입력


외부에서 접속을 허용하려면 `--host 0.0.0.0` 입력

vscode를 쓸 때 익스텐션을 설치 [Svelte for VS Code](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode).

## 배포 버젼으로 빌드하기

앱에 최적화된 버전을 만들기

```bash
npm run build
```

배포 버젼 실행하기

```bash
npm run start
```


## 싱글페이지 모드

single-page app (SPA) 모드로 빌드하고 싶을 때는 package.json의 start script를 아래 처럼 수정해서 사용

```js
"start": "sirv public --single"
```

## 웹 배포하기

### [Vercel](https://vercel.com) 사용해서 배포하기

vercel 설치하기

```bash
npm install -g vercel
```

아래 명령어로 배포하기

```bash
cd public
vercel deploy --name 프로젝트 이름
```
