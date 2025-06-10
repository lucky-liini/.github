---
name: 🧪 리펙토링 제보
about: 서비스에서 필요한 리펙토링을 간략히 적어주세요(명사형)
title: "[Refactor] "
labels: Refactor
assignees: ''

---
## 📖어느 코드에서 리펙토링이 필요한가요?
[어떤파일의 어떤부분인지 명사로 적기](https://github.com/myorg/myrepo/blob/main/src/index.js#L20)

## 💻 현 코드 기술 방법
기존 레거시 코드는 어떠한 코드인지 명사형으로 적기

## 🔍 왜 리펙토링이 필요한가요?
1. 이유1(하위에 코드스니펫으로 적어주면 best)
2. 이유2(또는 코드 링크 걸기)

### 📸 스크린샷 (선택사항)
이곳에 스크린샷


```
# 사용예시( 이 코드 블럭 전체를 지워주세요)

## 📖어느 코드에서 리펙토링이 필요한가요?
[src/pages/Register.vue의 setup 내부 로직](https://github.com/myorg/myrepo/blob/main/src/pages/Register.vue#L60)

## 💻 현 코드 기술 방법
모든 유효성 검사 로직이 `setup()` 안에 하드코딩돼 있어서 보기 힘들고 재사용도 어려움

## 🔍 왜 리펙토링이 필요한가요?
1. 다른 컴포넌트에서도 같은 유효성 검사 로직 반복됨  
   `js
   if (!email.includes('@')) { ... }
   `
2. 공통 훅(`useValidation`)으로 빼면 유지보수 쉬워짐

### 📸 스크린샷 (선택사항)
[첨부 예정]
```