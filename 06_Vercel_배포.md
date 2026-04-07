# 🚀 Step 3: Vercel로 배포하기

> **이 단계에서 할 일:** GitHub 저장소를 Vercel에 연결 → Deploy 클릭 한 번이면 끝! 환경변수 입력 없이 바로 됩니다.

---

## 1. Vercel에서 GitHub 저장소 연결하기

1. [vercel.com](https://vercel.com) 접속 → **GitHub 계정으로 로그인**

![Vercel 화면](screenshots/vercel_landing.png)

2. **"Add New Project"** 클릭
3. 저장소 목록에서 **`lunch-app`** 찾기 → **"Import"** 클릭

✅ **성공 확인:** 프로젝트 설정 화면이 열립니다.

---

## 2. 바로 Deploy!

빌드 설정 건드리지 말고 → **"Deploy"** 버튼 클릭!

> ✅ 환경변수 입력 없이 그냥 Deploy하면 됩니다.
> Step 2에서 GAS를 통해 Firebase 설정값을 코드에 직접 넣었기 때문이에요.

1~2분 후 **"Congratulations! 🎉"** 화면과 URL이 나타납니다.

---

## 3. Google 로그인 오류 방지 (배포 후 필수!)

1. Firebase 콘솔 → **"Authentication"** → **"Settings"** 탭
2. **"승인된 도메인"** → **"도메인 추가"**
3. Vercel URL 입력 (예: `lunch-app.vercel.app`) → **"추가"**

---

## 4. 팀에 공유하기

```
점심 신청 앱: https://lunch-app.vercel.app
Google 계정으로 로그인하면 바로 사용 가능합니다!
```

---

## 앱 수정할 때

GAS 채팅으로 수정 → GitHub 버튼으로 재커밋 → Vercel 자동 배포 (1~2분)

---

## ✅ Step 3 완료 체크

- [ ] Vercel에서 GitHub 저장소 Import
- [ ] Deploy 클릭 → 배포 성공 URL 확인
- [ ] Firebase 승인 도메인에 Vercel URL 추가
- [ ] 신청 화면 & 관리자 대시보드 동작 확인
- [ ] 팀에 URL 공유

---

**← [05_Google_로그인_세팅.md](./05_Google_로그인_세팅.md)** | **[README.md](./README.md) →**
