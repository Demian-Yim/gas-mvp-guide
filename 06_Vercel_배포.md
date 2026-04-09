# 🚀 Step 3: Vercel로 배포하기

> **이 단계에서 할 일:** GitHub 저장소를 Vercel에 연결 → Deploy 클릭 한 번으로 인터넷에 공개됩니다. 환경변수 입력 없이 바로 됩니다.

---

## 1. Vercel에서 GitHub 저장소 연결하기

1. [vercel.com](https://vercel.com) 접속 → **GitHub 계정으로 로그인**

![Vercel 화면](screenshots/step3_vercel_import_repo.png)
*↑ 로그인 후 이 화면에서 저장소를 선택하세요*

2. **"Add New Project"** 클릭
3. 저장소 목록에서 **내가 만든 저장소** (예: `lunch-cafe`) 찾기 → **"Import"** 클릭

✅ **성공 확인:** 프로젝트 설정 화면이 열립니다.

---

## 2. 바로 Deploy!

빌드 설정 건드리지 말고 → **"Deploy"** 버튼 클릭!

> ✅ 환경변수 입력 없이 그냥 Deploy하면 됩니다.
> Step 2에서 Firebase 설정값을 코드에 직접 넣었기 때문이에요.

1~2분 후 **"Congratulations! 🎉"** 화면과 URL이 나타납니다.

![배포 완료](screenshots/step3_vercel_success.png)
*↑ 이 화면이 나타나면 배포 성공! 표시된 URL이 내 앱 주소예요.*

> ※ URL은 Vercel이 자동 생성합니다. 예: `lunch-cafe-abc123.vercel.app` (사람마다 달라요)

---

## 3. Google 로그인 오류 방지 (배포 후 필수!)

1. Firebase 콘솔 → **"Authentication"** → **"Settings"** 탭

![Firebase 도메인 추가](screenshots/step3_firebase_domain.png)

2. **"승인된 도메인"** → **"도메인 추가"**
3. Vercel URL 입력 (예: `lunch-cafe-abc123.vercel.app`) → **"추가"**

> ⚠️ 이 단계를 빠뜨리면 Google 로그인이 차단됩니다. 반드시 해주세요!

---

## 4. 팀에 공유하기

```
🍱 점심 신청 앱 나왔습니다!

📱 앱 주소: https://[내 Vercel URL 붙여넣기]

Google 계정으로 로그인하면 바로 사용 가능합니다!
```

---

## 5. 앱 수정할 때

GAS 채팅으로 수정 → **Sync to GitHub** 버튼 → Vercel 자동 재배포 (1~2분)

---

## ✅ Step 3 완료 체크

- [ ] Vercel에서 GitHub 저장소 Import
- [ ] Deploy 클릭 → 배포 성공 URL 확인
- [ ] Firebase 승인 도메인에 Vercel URL 추가
- [ ] 신청 화면 & 관리자 대시보드 동작 확인
- [ ] 팀에 URL 공유

---

**← [05_Google_로그인_세팅.md](./05_Google_로그인_세팅.md)** | **[README.md](./README.md) →**
