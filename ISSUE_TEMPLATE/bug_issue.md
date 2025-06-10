---
name: 🐛 버그 제보
about: 서비스에서 발견된 버그를 간략히 적어주세요(명사형)
title: "[Bug] "
labels: Bug
assignees: ''

---

## 🧱 어떤 버그가 있나요?
어떤 버그인지 설명해주세요.

### 📸 스크린샷 (선택사항)
이곳에 스크린샷을 올려주세요

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
## 🧱 어떤 버그가 있나요?
게시글 목록 페이지에서 하단으로 스크롤을 내려도 새로운 게시글이 로딩되지 않고, 로딩 스피너만 무한히 표시됩니다.

### 📸 스크린샷 (선택사항)
![무한스크롤버그](https://user-images.githubusercontent.com/12345678/bug-example.png)

## 💻 재현 방법
- 문제 부분: [src/pages/PostList.vue의 89번째 줄](https://github.com/myorg/myrepo/blob/main/src/pages/PostList.vue#L89)
- 상황:
  1. 로그인 후 `/posts` 페이지로 이동
  2. 스크롤을 가장 아래까지 내림
  3. 로딩 아이콘이 계속 돌아가지만, 게시글이 추가로 로딩되지 않음

## 🔍 예상되는 원인은 무엇인가요?
1. `fetchMorePosts()` 호출 이후 응답이 실패하거나 `hasMore` 조건이 잘못 설정되어 있음
2. IntersectionObserver 콜백 내부에서 비동기 흐름이 중복 호출되며 race condition 발생 가능성 있음
```