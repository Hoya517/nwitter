# 김주호
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