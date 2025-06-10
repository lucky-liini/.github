---
name: ⚡️ 성능 저하 문제 제보
about: 서비스에서 발견된 성능 저하 문제를 간략히 적어주세요(명사형)
title: "[Performance] "
labels: Performance
assignees: ''

---

## 🧱 어떤 성능 문제가 있나요?
무엇이 잘못되었는지 설명해주세요.

## ⏳ 어느 만큼의 성능 문제가 있나요?
스크린샷이나 글씨로 적어주세요.(가능하면 스크린샷)  
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

## 🧱 어떤 성능 문제가 있나요?
대시보드 열 때, 차트랑 표 데이터 불러오는데 7초 이상 걸림

## ⏳ 어느 만큼의 성능 문제가 있나요?
- 평균 로딩 시간: 7.2초
- 기대값은 2초 이내
- 크롬/엣지 둘 다 동일하게 느림

### 📸 스크린샷 (선택사항)
![dashboard-delay](https://example.com/dashboard-delay.png)

## 💻 재현 방법
- 문제 부분: [src/pages/Dashboard.vue에서 mounted 이후 fetch](https://github.com/myorg/myrepo/blob/main/src/pages/Dashboard.vue#L33)
- 상황:
  1. 로그인 후 `/dashboard` 진입
  2. 화면이 늦게 뜸

## 🔍 예상되는 원인은 무엇인가요?
1. 차트 데이터 여러 개를 순차 요청하고 있음  
2. 불필요한 렌더링 로직이 섞여 있어서 첫 렌더링 느려짐
```