# 작성요령

##### 2024.08.13 윤지환 작성

---

### 0. 깃허브 레파지토리 Pull 받기

[깃허브]

<br/>
<br/>

### 1. docs 폴더 내 파일명 작성.

- 파일명은 자유롭게 입력. 확장자는 md 준수.
- ex) sample.md
- docs폴더내 md파일 하나하나가 게시글이라고 인지.

```
docs
|- sample.md
```

<br/>
<br/>

### 2. 페이지 최상단에 아래 내용 적용 (`---`포함)

```
---
title: Tutorial
description: This is a tutorial
layout: default
---
```

- title은 사용자에게 보여질 제목.
- description은 검색시 옆에 작게 보이는 설명란
- layout default 고정
- 이하 내용은 마크다운 양식으로 작성 (<i>레드마인은 플레인텍스트 사용이므로 문법이 다름.</i>)
- [마크다운]

<br/>
<br/>

### 3. 페이지 자식으로 나누기

```
부모페이지
---
title: 부모페이지1
description: This is a 부모페이지
layout: default
has_children: true
---
```

위와 같이 부모 페이지는 `has_children: true` 추가

```
자식페이지
---
title: 자식페이지1
description: This is a 자식페이지
layout: default
parent: 부모페이지1
---
```

자식 페이지는 위와 같이 `parent에 부모페이지 title 작성`

현재 최대 3Deps까지 지원.

<br/><br/>

### 4. 배포

- 작업완료 후 깃허브 레포지토리에 push하면 3분 내외로 실제 서버에 반영됨.
- 기타 템플릿 [메뉴얼] 확인

[깃허브]: https://github.com/iVH-Suite/iVH-Suite.github.io
[마크다운]: https://namu.wiki/w/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4
[메뉴얼]: https://just-the-docs.com/
