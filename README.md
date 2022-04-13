# 김주호
## [04월 13일]
#### 파이어베이스 로그인 설정
- 파이어베이스 인증 설정
- 이메일, 비밀번호 로그인 설정
- 구글, 깃허브 소셜 로그인 설정
- Auth.js에 로그인 폼 기본 구조 만들기
- 로그인 폼이 상태를 업데이트하도록 만들기
    - `useState` 로 함수 상태 만들기
    - `onChange`: 입력 시도중인지 판단
    - `onSubmit`

## [04월 06일]
#### 라우터 적용하기
- useState() 사용해서 로그인 여부에 따른 페이지 렌더링
```
isLoggedIn ? Auth(로그인 페이지) : Home(로그인 후 홈)
```
- App 컴포넌트에서 AppRouter 컴포넌트 렌더링
#### 파이어베이스 로그인 준비하기
- footer 추가
- useState 함수 위치 이동 (구조 분해 할당)
- jsconfig.json 절대 경로 적용
- 컴포넌트 import 경로 수정
- `npm install'로 설치한 패키지와 `.js`파일과 일치하면 안됨.
- 파이어베이스 인증 모듈 사용
## [03월 30일]
#### Firebase
- 파이어베이스 프로젝트 만들기
- 파이어베이스에 웹 애플리케이션 등록하기
- firebaseConfig값 복사하고 firebase.js 파일 수정하기
    - 파이어베이스 SDK 리액트 버전 설치
    ```
    npm install firebase
    ```
    - "firebase/app"에 포함된 모든 모듈을 firebase 객체에 부여
    ```
    import firebase from "firebase/app"         #firebase v8
    import firebase from "firebase/compat/app"  #firebase v9
    ```
#### Firebase
- .env 파일 생성
- .env 파일 숨기기: `.gitignore 에 추가`
- firebase.js에 환경 변수 적용

#### Router
- Router는 `BASE_URL/a`나 `BASE_URL/a`와 같은 주소 입력시, 어떤 컴포넌트(화면)를 보여줄지(렌더링) 결정하는 역할
- 뼈대 만들기
    - /src/`components` 생성
    - /src/`routes` 생성
- react-router-dom 설치하고 라우터 설정하기
```
npm install react-router-dom
```
- Component는 화면을 표현하기 위한 조각
- 훅스(Hooks)는 함수 컴포넌트에서 상태를 사용
-  useState()는 훅스(Hooks)를 사용
## [03월 23일]
#### CRA
-  프로젝트 생성
    ```
    cd /생성할 디렉토리
    npx create-react-app nwitter
    ```
-  깃허브 저장소와 nwitter 폴더 연결하기
    ```
    git remote add origin https://github.com/Hoya517/nwitter
    ```
- 기초 파일 수정
    - package.json, index.js, App.js
- 불필요한 파일 삭제
    - App.css, App.test.js, index.css, logo.svg, reportWebVitals.js
    - setupTest.js
- 깃허브에 파일 올리기
    ```
    git add.
    git commit -m '커밋내용'
    git push origin master
    ```
## [03월 16일]
#### 환경설정
##### node.js 설치
- node.js 공싱 홈페이지에서 다운
- homebrew 설치
    ```
    brew install node
    ```
- 버전 확인
    ```
    node -v  #node.js 버전
    npm -v   #node package manager 버전
    ```

##### npx 설치 
- npx는 설치할 노드 패키지를 최신 버전으로 다운로드해 설치한 다음 데스크톱에 남기지 않고 삭제함.
    ```
    npm install npx -g
    ```
- vsc 설치
- git 설치

##### 깃허브 저장소 만들기
- Repository name: nwitter
- Public