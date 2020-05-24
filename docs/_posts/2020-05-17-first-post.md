---
title: 정적 페이지 생성
author: devquint
show_author_profile: true
tags: TeXt, markdown
---

[TeXt 테마](https://github.com/kitian616/jekyll-TeXt-theme)를 사용했습니다.
해당 내용들은 관련 [문서](https://tianqi.name/jekyll-TeXt-theme/docs/en/quick-start)에 정리되어 있습니다.

### 상태 강조

성공
{:.success}

정보
{:.info}

경고
{:.warning}

에러
{:.error}

으로 표시 가능합니다.


### 태그

`성공`{:.success}
`정보`{:.info}
`경고`{:.warning}
`에러`{:.error}

등의 작은 태깅도 가능합니다.


### 이미지

border, shadow, rounded, circle 태그를 활용할 수 있습니다.

```markdown
![대체 텍스트](이미지 경로){:.circle.shadow}
```
![이미지](https://raw.githubusercontent.com/kitian616/jekyll-TeXt-theme/master/docs/assets/images/image.jpg){:.circle.shadow}


### 동영상

유튜브 등의 동영상 역시 가능합니다
자세한 내용은 [공식 문서](https://tianqi.name/jekyll-TeXt-theme/docs/en/extensions)에 있습니다.

```markdown
<div>{%- include extensions/youtube.html id='wbY97-hdD5c' -%}</div>
```
<div>{%- include extensions/youtube.html id='wbY97-hdD5c' -%}</div>
