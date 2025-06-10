---
name: 🧊 비기능적 불충족 문제
about: 비기능적 요구사항에서 어떠한 문제가 있는지 간략히 설명해주세요(명사형)
title: "[Non-functional] "
labels: Non-functional
assignees: ''

---

## 🧱 어떤 문제가 있나요?
- ??? : 아래 중에서 하나 골라서 설명해 주세요
```
🔐 보안 (Security)	인증, 권한, 데이터 보호
⚙️ 신뢰성 (Reliability)	장애 발생 시 복구 능력, 안정성
🧩 확장성 (Scalability)	부하 증가 시 대응 능력
🔄 이식성 (Portability)	OS, 브라우저, 장치 간 호환성
```
- 위에서 정한 문제대로 자세히 서술해주세요.

### 📸 스크린샷 (선택사항)
이곳에 스크린샷

## 💻 재현 방법
- 문제 부분: [어떤파일의 어떤부분인지 명사로 적기](https://github.com/myorg/myrepo/blob/main/src/index.js#L20)
- 상황:
  1. 어떤 상황에서 발생하는지
  2. 순서대로 작성해주세요.

## 🔍 예상되는 원인은 무엇인가요?
1. 예상되는 원인1
2. 예상되는 원인2


```
# 사용예시( 이 코드 블럭 전체를 지워주세요)

## 🧱 어떤 문제가 있나요?
- 🔄 **이식성 (Portability)**  
- iOS Safari 브라우저에서 회원가입 버튼이 클릭되지 않음. Chrome, Android 브라우저에서는 정상 작동. 브라우저 간 호환성이 부족한 상태.

### 📸 스크린샷 (선택사항)
![ios-button-fail](https://example.com/screenshot.png)

## 💻 재현 방법
- 문제 부분: [src/components/RegisterForm.vue의 버튼 이벤트 바인딩](https://github.com/myorg/myrepo/blob/main/src/components/RegisterForm.vue#L72)
- 상황:
  1. iPhone Safari 브라우저에서 회원가입 페이지 진입
  2. 폼 작성 후 "가입하기" 버튼을 터치
  3. 아무 동작도 일어나지 않음

## 🔍 예상되는 원인은 무엇인가요?
1. `@click` 대신 `@touchend` 이벤트가 필요한 환경에서 발생한 호환성 문제
2. `preventDefault()`로 인해 iOS 터치 이벤트가 제대로 전파되지 않음
```