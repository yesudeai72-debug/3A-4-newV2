# 분짜 요리 어휘 · 한국어 3A

분짜 조리 장면을 통해 한국어 요리 동사 7개를 익히는 정적 웹앱입니다.

## 실행

`index.html`을 웹 브라우저로 열면 됩니다. 학습 결과를 저장하려면 아래 Firebase 설정을 완료해야 합니다.

## Firebase 설정

1. Firebase Console에서 새 프로젝트와 웹 앱을 만듭니다.
2. **Authentication**에서 익명 로그인을 사용 설정합니다.
3. **Realtime Database**를 만들고, 처음에는 잠금 모드를 선택합니다.
4. `firebase-config.js`의 `YOUR_...` 값을 웹 앱 구성 값으로 바꿉니다.
5. `database.rules.json`의 내용을 Realtime Database의 Rules 화면에 붙여 넣고 게시합니다.

학생 웹앱은 `learningResults`에 새 기록만 만들 수 있으며, 읽기·수정·삭제는 허용하지 않습니다. 교사는 Firebase Console에서 전체 기록을 확인합니다.

## GitHub Pages 배포

이 폴더를 새 GitHub 저장소에 올린 뒤, GitHub의 **Settings → Pages**에서 `main` 브랜치와 `/(root)`를 선택하면 됩니다.

## 구성

- `index.html`: 학습·복습 화면
- `assets/`: 7개 이미지와 도입 영상
