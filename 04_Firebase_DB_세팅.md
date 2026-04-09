# 🔥 Step 2: Firebase — 데이터 저장소 & GAS에 설정값 붙여넣기

> **이 단계에서 할 일:** Firebase를 만들고, 설정값을 AI Studio에 붙여넣으면 끝! Vercel에 따로 환경변수를 입력할 필요가 없어요.

Firebase는 Google이 제공하는 **무료 백엔드**입니다. 서버 없이 데이터를 저장할 수 있어요.

---

## 1. Firebase 프로젝트 만들기

1. [console.firebase.google.com](https://console.firebase.google.com) 접속
2. Google 계정으로 로그인
3. **"프로젝트 추가"** 클릭

![Firebase 콘솔](screenshots/step2_firebase_new_project.png)
*↑ 이 화면에서 "프로젝트 추가"를 클릭하세요*

4. 프로젝트 이름 입력 (예: `lunch-cafe`)
5. Google Analytics → **"지금은 사용 안 함"** 선택
6. **"프로젝트 만들기"** → 완료 후 **"계속"** 클릭

✅ **성공 확인:** 프로젝트 대시보드 화면이 나타납니다.

---

## 2. Firestore 데이터베이스 만들기

1. 좌측 메뉴 → **"빌드"** → **"Firestore Database"** 클릭
2. **"데이터베이스 만들기"** 클릭

![Firestore 활성화](screenshots/step2_firebase_firestore.png)
*↑ "데이터베이스 만들기" 클릭*

3. **"테스트 모드로 시작"** 선택 → **"다음"** 클릭
4. 위치: **`asia-northeast3 (서울)`** 선택 → **"완료"** 클릭

✅ **성공 확인:** "데이터" 탭이 있는 Firestore 화면이 보입니다.

---

## 3. 앱 등록 & 설정값 복사

1. 좌측 상단 **톱니바퀴(⚙️)** 클릭 → **"프로젝트 설정"**
2. 아래 스크롤 → **"내 앱"** → 웹 아이콘 **`</>`** 클릭
3. 앱 닉네임 입력 (아무 이름이나 OK) → **"앱 등록"**
4. 아래 코드 블록 전체를 **복사**

![Firebase 설정값](screenshots/step2_firebase_config.png)
*↑ firebaseConfig 전체 복사 (apiKey부터 appId까지)*

```
const firebaseConfig = {
  apiKey: "AIzaSy...",
  authDomain: "lunch-cafe.firebaseapp.com",
  projectId: "lunch-cafe",
  storageBucket: "lunch-cafe.appspot.com",
  messagingSenderId: "123...",
  appId: "1:123:web:abc..."
};
```

> ⚠️ 이 값은 예시입니다. 실제로는 **내 Firebase에서 복사한 값**을 사용하세요!

---

## 4. AI Studio에 설정값 붙여넣기 → GitHub 재커밋

1. **AI Studio Build 탭으로 돌아가서** 채팅창에 입력:

```
Firebase 설정값을 아래로 교체해줘.

(복사한 firebaseConfig 붙여넣기)
```

2. AI가 코드에 값을 채워 넣으면 **"Sync to GitHub"** 버튼 클릭 → GitHub에 자동 업데이트

> 💡 이렇게 하면 Vercel에서 환경변수를 따로 입력할 필요가 없어요!

---

## ✅ Step 2 완료 체크

- [ ] Firebase 프로젝트 생성
- [ ] Firestore Database 활성화 (테스트 모드, 서울)
- [ ] 앱 등록 → firebaseConfig 복사
- [ ] GAS에 붙여넣기 → Sync to GitHub 완료

---

**다음 단계 →** [05_Google_로그인_세팅.md](./05_Google_로그인_세팅.md)
